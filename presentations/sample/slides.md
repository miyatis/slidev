---
theme: seriph
background: https://cover.sli.dev
title: Slidev サンプルプレゼンテーション
info: |
  ## Slidev マルチプレゼンテーション環境
  pnpm workspaces を使った複数プレゼンテーション管理のサンプルです。
class: text-center
drawings:
  persist: false
transition: slide-left
---

# Slidev サンプルプレゼンテーション

pnpm workspaces による マルチプレゼンテーション環境

<div class="abs-br m-6 flex gap-2">
  <a href="https://sli.dev" target="_blank" class="text-xl slidev-icon-btn">
    Slidev Docs
  </a>
</div>

---
transition: fade-out
---

# 目次

このサンプルでは Slidev の主要機能を紹介します

- **Markdown ベース** - スライドを Markdown で記述
- **テーマ対応** - テーマを簡単に切り替え
- **コードハイライト** - シンタックスハイライト付きコード表示
- **LaTeX 数式** - KaTeX による数式レンダリング
- **レイアウト** - 豊富なビルトインレイアウト
- **アニメーション** - クリックアニメーション対応

---

# Markdown 記法

Slidev ではおなじみの Markdown 記法がそのまま使えます

テキストを **太字** や *斜体* にしたり、[リンク](https://sli.dev) を埋め込めます。

> 引用ブロックも使えます

### リスト

- アイテム 1
- アイテム 2
  - ネストも可能
- アイテム 3

### テーブル

| 機能 | 対応状況 |
|------|---------|
| Markdown | ✅ |
| コードハイライト | ✅ |
| LaTeX | ✅ |

---

# コードハイライト

シンタックスハイライト付きでコードを表示できます

```ts {all|1-3|5-8|all}
// TypeScript のコード例
interface User {
  name: string
  age: number
}

function greet(user: User): string {
  return `Hello, ${user.name}!`
}

const user: User = { name: 'Slidev', age: 1 }
console.log(greet(user))
```

行のハイライトやステップ表示にも対応しています。

---

# LaTeX 数式

KaTeX を使った数式レンダリング

インライン数式: $E = mc^2$

ブロック数式:

$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

$$
f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

---
layout: two-cols
layoutClass: gap-16
---

# 2カラムレイアウト

`two-cols` レイアウトで左右に分割できます。

左カラムにはテキストを配置し、右カラムにはコードやリストなどを表示できます。

::right::

### 右カラム

```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

for i in range(10):
    print(fibonacci(i))
```

---
layout: center
class: text-center
---

# ありがとうございました

[Slidev ドキュメント](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev)
