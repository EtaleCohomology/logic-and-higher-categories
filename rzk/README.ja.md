[English](./README.md) | [日本語](./README.ja.md)

# Rzk：総合的な∞-圏論、Rezk 型、米田の補題

∞-圏論のためだけに作られた定理証明言語 **Rzk** についての記事を集めたフォルダーです。Rzk は、Emily Riehl と Michael Shulman が 2017 年に提案した単体的型理論（RSTT）を実装した言語で、Nikolai Kudasov が設計・実装しました。

## 記事の一覧

| フォルダー | 記事 | Qiita |
|---|---|---|
| [01-synthetic-infinity-categories](./01-synthetic-infinity-categories/) | ∞-圏論のためだけに作られた定理証明言語 Rzk ―― extension type から、∞-圏を表す Rezk 型、そして米田の補題まで（PDF） | [Qiita](https://qiita.com/etale_cohomology/items/e9d3d0d6cc099b59c3d1) |

## 01 ── ∞-圏論のためだけに作られた定理証明言語 Rzk

📄 [rzk_infinity_categories_JA.pdf](./01-synthetic-infinity-categories/rzk_infinity_categories_JA.pdf)（日本語、172ページ）

2023 年、数学者の Emily Riehl は「∞-圏論を、学部生に教えられるか？」と問いかけました。本稿は、その問いへの技術的な回答のひとつとして、Rzk をたどります。汎用の定理証明言語で「x から y への射」を素朴に定義すると、両端が x と y であることの証拠を２つ持ち回ることになり、可換三角形や可換四面体では、証拠がさらに増えていきます。Rzk では、extension type によって両端の条件が型そのものに埋め込まれるので、恒等射の可換三角形は、本体が１行の定義になります。

### 内容

1. 汎用の言語と、専用の言語（Lean、Agda、Rocq と Rzk、名前の由来、開発の経緯）
2. ∞-圏とは何か（圏、高次の射、(∞,1)-圏と (∞,0)-圏、なぜ型理論で扱いたいのか）
3. 汎用の言語で素朴に書くと、何が起きるか
4. Rzk の３つの層（cube、tope、shape、extension type）
5. 射と可換三角形を書く（hom 型、hom2 型、恒等射の可換三角形）
6. Segal 型と Rezk 型（∞-圏そのもの）
7. 実際に、何が証明されたのか（sHoTT ライブラリ、∞-圏論の米田の補題、教育での使用、tope solver の実測）
8. Rzk が RSTT に加えた改良（split extension types、coercion-free subtyping、first-class parameters、tope solver の自動化、双方向型検査）
9. 理論と実装の往復（忠実性、保存性、規則を書き下したことで見つかった２つの健全性のバグ）
10. 分野専用の言語という設計（強みと弱み、今後の課題、「学部生に教えられるか」への回答）

付録 A：本稿で扱った用語（22語）。付録 B：参考文献。

### 想定読者

- Haskell を学び始めた方
- 圏論の学習を始めたばかりの方
- 定理証明支援系に関心のある方
- 型システムの設計に関心のある方

圏論、∞-圏、ホモトピー型理論の知識は前提としません。必要な前提は、すべて本文で説明しています。

### Rzk を試す

Rzk は、インストールなしにブラウザで動かせます：https://rzk-lang.github.io/rzk/playground/

記事の中のコードの例は、筆者が Rzk 0.11.4 で動作を確かめたものです。

### 主な出典

- E. Riehl, M. Shulman. "A type theory for synthetic ∞-categories." Higher Structures, 1(1), 147–224, 2017.
- N. Kudasov, E. Riehl, J. Weinberger. "Formalizing the ∞-categorical Yoneda lemma." CPP 2024.
- E. Riehl. "Could ∞-category theory be taught to undergraduates?" Notices of the AMS, 2023年5月号.
- Rzk：https://github.com/rzk-lang/rzk
- sHoTT ライブラリ：https://github.com/rzk-lang/sHoTT

参考文献の全体は、記事の付録 B にあります。

## ライセンス

CC BY 4.0
