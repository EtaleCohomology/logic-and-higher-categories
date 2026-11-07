[English](./README.md) | [日本語](./README.ja.md)

# Rzk: synthetic ∞-categories, Rezk types and the Yoneda lemma

Articles on **Rzk**, a proof assistant designed specifically for ∞-category theory. Rzk implements the simplicial type theory (RSTT) proposed by Emily Riehl and Michael Shulman in 2017, and was designed and implemented by Nikolai Kudasov.

## Articles

| Folder | Article | Qiita |
|---|---|---|
| [01-synthetic-infinity-categories](./01-synthetic-infinity-categories/) | Rzk, a theorem-proving language made only for ∞-category theory: from extension types to Rezk types and the Yoneda lemma (Japanese, PDF) | [Qiita](https://qiita.com/etale_cohomology/items/e9d3d0d6cc099b59c3d1) |

## 01 — Rzk, a theorem-proving language made only for ∞-category theory

📄 [rzk_infinity_categories_JA.pdf](./01-synthetic-infinity-categories/rzk_infinity_categories_JA.pdf) (Japanese, 172 pages)

Emily Riehl asked in 2023 whether ∞-category theory could be taught to undergraduates. This article follows Rzk as one technical answer to that question. In a general-purpose proof assistant, a morphism from x to y has to carry two pieces of evidence that its endpoints are x and y, and the evidence multiplies for commutative triangles and tetrahedra. In Rzk, the endpoint conditions are built into the type itself through extension types, so the identity commutative triangle becomes a one-line definition.

### Contents

1. General-purpose languages and a dedicated language (Lean, Agda, Rocq and Rzk; the origin of the name; the development history)
2. What an ∞-category is (categories, higher morphisms, (∞,1)- and (∞,0)-categories, why type theory)
3. What goes wrong when written naively in a general-purpose language
4. The three layers of Rzk (cubes, topes, shapes and extension types)
5. Writing morphisms and commutative triangles (hom and hom2 types, the identity triangle)
6. Segal types and Rezk types (∞-categories themselves)
7. What has actually been proved (the sHoTT library, the ∞-categorical Yoneda lemma, teaching use, tope-solver performance)
8. What Rzk added to the paper theory (split extension types, coercion-free subtyping, first-class parameters, an automated tope solver, bidirectional type checking)
9. Going back and forth between theory and implementation (faithfulness, conservativity, two soundness bugs found by writing the rules down)
10. The design of a domain-specific language (strengths and weaknesses, open problems, an answer to "can it be taught to undergraduates?")

Appendix A: 22 terms used in the article. Appendix B: references.

### Intended readers

- People who have started learning Haskell
- People who have just started learning category theory
- People interested in proof assistants
- People interested in the design of type systems

No prior knowledge of category theory, ∞-categories or homotopy type theory is assumed; everything needed is explained in the text.

### Try Rzk

Rzk runs in the browser, with no installation: https://rzk-lang.github.io/rzk/playground/

The code examples in the article were checked by the author with Rzk 0.11.4.

### Key sources

- E. Riehl, M. Shulman. "A type theory for synthetic ∞-categories." Higher Structures, 1(1), 147–224, 2017.
- N. Kudasov, E. Riehl, J. Weinberger. "Formalizing the ∞-categorical Yoneda lemma." CPP 2024.
- E. Riehl. "Could ∞-category theory be taught to undergraduates?" Notices of the AMS, May 2023.
- Rzk: https://github.com/rzk-lang/rzk
- The sHoTT library: https://github.com/rzk-lang/sHoTT

The full reference list is in Appendix B of the article.

## License

CC BY 4.0
