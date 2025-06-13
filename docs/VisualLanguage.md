
---

# 📘 `docs/VisualLanguage.md` – Visual Language Spec for **Monadrift**

```markdown
# Monadrift Visual Language Guide

Monadrift uses a specialized set of visual terms to represent Haskell constructs in a meaningful and interactive way. This guide explains what each visual element represents, and how it maps to actual Haskell code structures.

---

## 🧩 Core Terminology

| Visual Term          | Abstract Term | Haskell Construct               | Notes                                                               |
| -------------------- | ------------- | ------------------------------- | ------------------------------------------------------------------- |
| **Function card**    | `Node`        | `f :: A -> B` or `A -> m B`     | All individual functions: pure, effectful, conditional, etc.        |
| **Conditional fork** | `Node`        | `guard`, `case`, `Either`, etc. | Also represented as a `Node`, with logic implied by naming and type |
| **Link**             | `Link`        | `f . g`, `>>=`, `<*>`, etc.     | Connection between nodes (composition, bind, etc.)                  |
| **Linear flow**      | `Pipe`        | Chained function application    | Represents a sequence of `Node`s; a linear data transformation flow |
| **Group of nodes**   | `Group`       | Module or logical cluster       | A named or thematic collection of related `Node`s                   |
| **Full canvas**      | `Workspace`   | Entire program or feature flow  | The entire visual/functional scope — one full user story or system  |
| **Context wrapper**  | `Envelope`    | `Maybe`, `IO`, `Either`, etc.   | A value inside a computational context (Monad/Functor/Applicative)  |

---

## 🖼️ Visual Examples (Textual)

### Example 1: A simple composition

```haskell
processData = parse >=> validate >=> format

