# 🌀 SpellShape: A Lightweight AI-Native Format for Parametric 3D

**SpellShape** is an evolving idea — a lightweight, text-based format for defining parametric 3D models that are easy to automate, modify, and generate with AI.

Unlike traditional formats that store final geometry, `.spell` aims to capture the **logic** behind a model: its parameters, rules, relationships, and expressions.

This repo is home to the draft schema, core principles, and example files — and it's all **actively in development**.

## ✨ Why a New Format?

Over the years, we've seen formats like:

- **OBJ / STL** – simple geometry, no logic
- **glTF / GLB** – great for delivery, not for editing
- **STEP / IGES** – parametric, but locked into engineering workflows
- **X3D / VRML** – expressive but bloated and outdated
- **USD (Universal Scene Description)** – powerful parametric capabilities but complex and heavy for simple use cases

None of these are designed for:

- 🔁 **Reusable parametric models**
- 🧠 **LLM generation / editing**
- ⚙️ **Cross-platform automation**
- ✍️ **Human-readable, declarative logic**

That's the gap `.spell` tries to explore.

## 🧠 What is `.spell`?

A `.spell` file is a structured JSON document describing a **parametric 3D object** or scene.

This includes:

- Parameters and expressions  
- Geometry templates (e.g. `box`, `cylinder`)  
- Scene hierarchy  
- Basic controls for editing  
- Optional logic (repeaters, constraints)

### 🧪 Example (Work-in-Progress)

```json
{
  "type": "box",
  "dimensions": ["width", "height", "depth"],
  "position": [0, "height/2", 0],
  "parameters": {
    "width": 1.0,
    "height": 2.0,
    "depth": 0.5
  }
}
```

This is not a final spec — just one possible way to represent procedural logic in a readable, generative format.

## 🔍 Goals & Questions

This project is not about final answers — it's about exploration.

We're asking:

- What does a LLM-native 3D format look like?
- How much logic can fit in a readable file?
- Can one format span design, web, CAD, and AI?
- What's the minimal structure needed to support real procedural workflows?

## 🧩 Current Experiments

- 📄 **Schema design and constraints**
- 🧪 **Three.js parser** (early prototype)
- 🧠 **Prompt-to-model generation** via LLM
- 🧱 **Templates and component reuse**
- 🧰 **Visual editor concepts** (WIP)

## 🛠 Related Repos (All in Progress and Coming Soon)

| Repo | Purpose |
|------|---------|
| `spellshape-three` | Parser for Three.js runtime |
| `spellshape-web` | Experimental online editor |
| `spellshape-examples` | Early test models |

## 🧑‍🤝‍🧑 How to Get Involved

If you care about:

- **Parametric design**
- **AI and generative 3D**
- **Web-first design tools**
- **Open source schemas and standards**

…then we'd love your input, critiques, ideas, or experiments.

This is early-stage and highly collaborative. Please open an issue or join the discussion.

## 📚 Background Reading

- Format comparison: OBJ, glTF, X3D, STEP vs. .spell
- Design goals for AI-native 3D modeling
- Blog post: What makes a format LLM-friendly?

*(links coming soon)*

## 📝 License

MIT License — open and free for experimentation.

## ✉️ Contact

Questions? Ideas? Use cases?

→ stepan.kukharskiy@gmail.com  
→ GitHub issues  
→ More coming soon at spellshape.com  

**This is a living spec — not a finished product.**

If you're building the future of AI-native 3D design, let's build together.
