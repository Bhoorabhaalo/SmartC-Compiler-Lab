# SmartC Compiler Lab — Lex + LL(1) Parser

> **Live Demo → [smartc-compiler-lab.vercel.app](https://smartc-compiler-lab.vercel.app)** *(update this link after first deploy)*

A visually rich, browser-based Compiler Design lab project that demonstrates a **C-like compiler front-end** — built with pure HTML, CSS, and JavaScript. No backend. No build step.

---

## ✨ Features

| Phase | What it does |
|---|---|
| **Source Code Editor** | Write C-Lite code with live character count & line numbers |
| **Lex-inspired Tokenizer** | Scans code and produces a typed token stream |
| **Token Stream Table** | Displays every lexeme, token type, and category |
| **LL(1) Predictive Parser** | Validates syntax using a top-down, 1-lookahead approach |
| **Parser Stack Trace** | Shows every push/pop step of the parsing process |
| **Compiler Console** | Real-time diagnostics and error messages |
| **Grammar Panel** | The full LL(1) grammar used for parsing |
| **Compiler Insights** | Quick stats: token count, identifiers, operators, syntax status |

---

## 🛠 Technologies

- HTML5 · CSS3 · Vanilla JavaScript
- **No npm, no framework, no build step**
- Deployable to any static host (Vercel, GitHub Pages, Netlify, …)

---

## 🚀 Run Locally

```bash
# Clone the repo
git clone https://github.com/<your-username>/SmartC_Compiler_Lab_PREMIUM_TEAM_UI.git
cd SmartC_Compiler_Lab_PREMIUM_TEAM_UI

# Open in browser (double-click or use VS Code Live Server)
open index.html
```

Or install the **Live Server** VS Code extension, right-click `index.html` → **Open with Live Server**.

---

## ☁️ Deploy to Vercel

### Option A — Vercel CLI (recommended)
```bash
npm i -g vercel
vercel
```
Follow the prompts — the `vercel.json` in this repo already configures everything.

### Option B — Vercel Dashboard
1. Push this repo to GitHub.
2. Go to [vercel.com/new](https://vercel.com/new).
3. Import the GitHub repo.
4. Framework Preset: **Other** (or leave as Static).
5. Click **Deploy** — done in ~30 seconds.

---

## 📄 Supported C-Lite Syntax

```c
int main() {
    int a = 10;
    int b = 20;
    int sum = a + b;

    if (sum > 20) {
        print(sum);
    }

    return 0;
}
```

Supports: `int`, variable declarations, assignments, arithmetic, `if` blocks, `print(...)`, `return`, and relational operators (`> < == != >= <=`).

---

## 🎓 Lab Viva Notes

**LEX phase:** Converts source characters into tokens — `KEYWORD`, `ID`, `NUM`, `OP`, `DELIMITER`.

**LL(1) phase:** Top-down predictive parsing. First `L` = left-to-right scan; second `L` = leftmost derivation; `1` = one lookahead token used to choose productions.

### Demo flow
1. Load the sample or write your own code.
2. Click **Compile & Visualize**.
3. Walk through the Token Stream table.
4. Explain the Parser Stack Trace step by step.
5. Show **ACCEPT** result.
6. Introduce a syntax error (e.g. `sum >` with no RHS) and recompile.
7. Point out the error message in the console.
8. Discuss the Grammar panel and why LL(1) is used.

---

## 👥 Team

| Name | Role |
|---|---|
| **Vipul Sharma** | Developer · UI & Integration |
| **Vinayak Goyal** | Developer · Compiler Logic |
| **Vivek Kumar** | Developer · Documentation |

---

## 📜 License

Released for educational use. MIT License.
