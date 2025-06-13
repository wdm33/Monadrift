# Monadrift
Haskell IDE

**Monadrift** is a visual, AI-assisted Haskell IDE that lets you explore and build your codebase as an interactive network of functions. Rather than navigating flat source files, you work with **Nodes**, **Links**, and **Pipes**—logical, composable units that mirror how Haskell works at its core.

### 🌟 Key Features

- 🧠 **AI-enhanced function editing**
- 🧩 **Drag-and-drop Nodes**
- 🔗 **Visual composition with links and pipelines**
- 📦 **Context-aware envelopes** (`IO`, `Maybe`, `Either`, etc.)
- 🧪 **Inline type inference, summaries, test suggestions**

---

### 🧠 Visual Language

Monadrift introduces a functional-visual vocabulary to bridge Haskell structure with visual clarity:

| Visual Term       | Haskell Construct         | Description                                   |
|-------------------|---------------------------|-----------------------------------------------|
| **Node** | `f :: A -> B`             | An individual function, visualized as a node  |
| **Link**          | `f . g`, `>>=`, `<*>`     | Compositional connection between nodes        |
| **Pipe**          | `f x -> g x -> h x`       | A linear flow of transformations              |
| **Group**         | Module or feature cluster | A visual collection of related nodes          |
| **Envelope**      | `IO`, `Maybe`, `Either`   | A wrapper showing contextual computation      |
| **Workspace**     | Entire program view       | The full canvas for building your system      |

📘 **[See full spec → `docs/VisualLanguage.md`](docs/VisualLanguage.md)**

---

### 🚀 Getting Started

```bash
git clone https://github.com/yourname/monadrift.git
cd monadrift
# Follow setup instructions for backend/frontend

