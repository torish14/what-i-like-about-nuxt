---
# try also 'default' to start simple
theme: vuetiful
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# ドキュメントを翻訳してみて改めてわかった Nuxt のいいところ💚

Nuxt 3 の優れた開発者体験を紐解く

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Next <carbon:arrow-right class="inline"/>
  </span>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# ところで、あなただれ？

<p>
	<img src="ponpo-san.png" alt="映画大好きポンポさん">
</p>

[torish14_str - Twitter](https://twitter.com/torish14_str)

- 📛 **Name** - torish14（トリッシュ）
- 💼 **Career** - 独学 → ハッカソン優勝 → フリーランスエンジニア → 法人の代表兼エンジニア
- 🧑‍💻 **Now Working** - 性教育アプリの開発
- 💚 **Love** - パフォーマンスチューニングと UX デザイン
- 📖 **Learning** - 低レイヤー

[ハッカーと話そう | ハッカー飯](https://hackermeshi.com)

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
img {
	border-radius: 50%;
	height: 100px;
	width: 100px;
}
</style>
<!-- <style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style> -->

---

# 🤔 どうして登壇しようと思ったか？

- はじめて Nuxt を触ったときから虜になった
- 純粋に Nuxt を広めたいと思ったから
- アウトプットすることで、改めて Nuxt の理解を深められると思ったから

---

# 👀 想定している視聴者

- Nuxt に興味があるけど、まだ使ったことがない初心者
- Nuxt 2 は使ったことがあるけど、Nuxt 3 はまだ使ったことがない中級者

---

# 🛣️ 今日のゴール

- まだ Nuxt を使ったことがない初心者に、Nuxt を主体的に使ってもらうこと！
- まだ Nuxt 3 に乗り換えられていない中級者に、Nuxt 3 を主体的に使ってもらうこと！

---

# 🚨 本題に入ります

---

# 📝 Nuxt 3 のドキュメント、翻訳してみました

- 基本的には、DeepL を使いました
- 訳がおかしいところは自分で修正
- まだまだ翻訳の途中です

[Nuxt 3 公式ドキュメント 日本語訳 - Zenn](https://zenn.dev/torish/scraps/16676a3500ad99)

---

# 改めてわかった Nuxt（Nuxt 3）のいいところ

---

# それは、、

---

# ズバリ、優れた開発者体験🥳

---

# 具体的には、

- 🔰 学習コストが低い
- ⚙️ 余計なセットアップが不要
- ⚡️ ホットリロードが高速
- 🤖 自動インポート機能
- 🕵️ TypeScript のサポート強化
- 💚 なにより開発していて楽しい

---

# ひとつずつ見ていきましょう！

---

# 🔰 学習コストが低い

- Vue のフレームワークで直感的に書ける
- React と比べてコード量が少ない

---

# ⚙️ 余計なセットアップが不要とは？

- TypeScript がすぐに使える（最高）
- CSS モジュールがすぐに使える
- 糖衣構文(`<script setup>`)も使える

---

# TypeScript がすぐに使えるとは？

拡張子を `.js` から `.ts` に変える。

```js
<script lang="ts">
</script>
```

これだけ。

---

# CSS モジュールがすぐに使えるとは？

```css
<style lang="scss">
</style>
```

これだけ。

---

# 糖衣構文とは？

プログラムの意味としては同じものをよりわかりやすい構文に書き換えたもの

- 記述量が減って簡潔になる
- props、emit を使うときに、純粋な TypeScript が使える
- ランタイムのパフォーマンスが上がる

```js
<script setup lang="ts">
</script>
```

Vue 3 を使っていないひとはぜひ使いましょう！

[【Vue.js 3.2】`<script setup>` 構文がすごくすごい - Zenn](https://zenn.dev/azukiazusa/articles/676d88675e4e74)

---

# ⚡ ホットリロードが高速とは？

- Vite がとにかく爆速
- `npm` や `yarn` はもちろんのこと `pnpm` も使える

---

# 🤖 自動インポート機能とは？

- components を明示的にインポートする必要がない
- composables を明示的にインポートする必要がない
- Vue API を明示的にインポートする必要がない
- ヘルパー関数を明示的にインポートする必要がない

[Nuxt 3 - Auto imports](https://v3.nuxtjs.org/concepts/auto-imports#auto-imports)

---

# 🕵️‍♂️ TypeScript のサポート強化とは？

- TypeScript がネイティブサポートになった
- 厳格モードも使える
- Volar のインストールをお忘れなく！
- `nuxi typecheck` で型チェック

[Nuxt 3 - TypeScript](https://v3.nuxtjs.org/concepts/typescript#typescript)

---

# もしかして、TypeScript を使ったことがない？

---

# TypeScript の簡単な特徴

- 🦸‍♂️ JavaScript の上位互換
- 😌 安全性が高い開発ができる
- 🧑‍🔬 型推論がある
- ✅ 開発者体験がよい

[今まで TypeScript をなんとなく書いてきたので、勉強し直す - Zenn](https://zenn.dev/torish/scraps/6922b791cdfff7)

---

# つまり、Nuxt 3 は開発していて本当に楽しい 🥳

- 余計なことを考える必要がない
- イライラすることが少ない
- 本質であるアプリ開発に集中できる

---

# まとめ

Nuxt 3 の優れた開発者体験を支える機能たち

- ⚙️ 余計なセットアップがいらないからラクちん
- ⚡ ホットリロードが高速だからイライラしない
- 🤖 自動インポート機能のおかげでスラスラコードが書けちゃう
- 🕵️‍♂️ TypeScript のサポート強化で型安全な開発ができちゃう
- 💚 開発していて本当に楽しい(いや、ほんと。)

---

# すこしでも Nuxt に興味が湧きましたか？

---

# ぜひ Nuxt を触ってみてね！


- [Nuxt 3 - Introduction](https://v3.nuxtjs.org/getting-started/introduction/)
- [Nuxt 3 - Installation](https://v3.nuxtjs.org/getting-started/installation)

エディタではじめるのがめんどさいなら、[StackBlitz](https://stackblitz.com/github/nuxt/starter/tree/v3-stackblitz) や [CodeSandbox](https://codesandbox.io/s/github/nuxt/starter/tree/v3-codesandbox) があるよ

参考にさせていただいたサイト

- [Nuxt 3 を今すぐオススメしたい 15 のポイント - Zenn](https://zenn.dev/ytr0903/articles/d0a91f6180d34e)
- [Nuxt 3 がパブリックベータ版になったので新機能の紹介や所感など - Zenn](https://zenn.dev/miruoon_892/articles/e06b1c7533d754df8a8c)
- [Nuxt 3 の新しい機能 - Zenn](https://zenn.dev/azukiazusa/articles/nuxt3-new-features)
