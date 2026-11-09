# AI Cost Per Task vs. Intelligence Score — Chart Visualizer 📊

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Chart.js](https://img.shields.io/badge/Chart.js-v4.4.1-orange.svg)](https://www.chartjs.org/)

An interactive visualization tool mapping LLM average cost-per-task against intelligence benchmark scores (**Artificial Analysis Intelligence Index v5.0**) across varying reasoning/thinking effort levels.

תרשים אינטראקטיבי להשוואת עלות ממוצעת למשימה אל מול ציון ביצועים ומדד אינטליגנציה עבור מודלי שפה מובילים ברמות חשיבה שונות (Artificial Analysis Intelligence Index v5.0).

---

## 🌟 Highlights

- **Logarithmic Cost Analysis**: Visualizes cost per task across wide ranges ($0.03 to $25+) on a logarithmic X-axis.
- **Reasoning Effort Breakdown**: Displays performance progression per model across thinking/effort levels (`low`, `medium`, `high`, `xhigh`, `max`).
- **Data Transparency**: Clear visual distinction between officially verified benchmark measurements (solid points) and mathematically extrapolated estimates (hollow points).
- **Interactive Controls**: Filter and toggle individual models dynamically; responsive data table updating in real time.
- **Zero-Dependency & Standalone**: Pure HTML/CSS/JavaScript with CDN-hosted Chart.js. No build steps, bundlers, or servers required.

---

## 🤖 Models Covered

| Provider / Family | Models |
|---|---|
| **Anthropic** | Claude Opus 5.5, Claude Sonnet 5.5, Claude Haiku 5.5, Claude Fable 5.2, Claude Fable 5.1, Claude Fable 5, Claude Opus 5 |
| **OpenAI** | GPT-6 Astra, GPT-6.1 Sol, GPT-6.1 Terra, GPT-6 Sol, GPT-5.6 Sol, GPT-5.6 Terra, GPT-5.6 Luna |
| **Google** | Gemini 4 Carbon, Gemini 4 Argon |
| **Zhipu AI** | GLM-5.3-Flash |

---

## 🚀 Quick Start / How to Run

Because this is a completely standalone single-page web app, you can run it in seconds:

### Option 1: Direct File
Simply clone the repository and double-click `index.html` in your file explorer, or open it in any modern browser.

### Option 2: Local Static Server
If you prefer running via a local server:

```bash
# Clone repository
git clone https://github.com/giamat13/ai-cost-per-task-charts.git
cd ai-cost-per-task-charts

# Using Python
python -m http.server 8000

# Or using Node.js / npx
npx serve .
```
Then navigate to `http://localhost:8000`.

---

## 🌐 Deploy to GitHub Pages

You can host this live for free in under a minute with GitHub Pages:

1. Push this repository to GitHub.
2. In your repo settings, go to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
4. Select `main` branch and `/ (root)` folder, then click **Save**.
5. Your interactive chart will be live at `https://<your-username>.github.io/<repo-name>/`.

---

## 📐 Methodology & Data Derivation

- **Measured in v5.0 (Artificial Analysis)**: Solid points represent verified, published benchmarks on Intelligence Index v5.0.
- **Extrapolated / Estimated Points**: Hollow points represent estimates derived using proportional multipliers and historical patterns from prior index releases (e.g. v4.3.2 and v4.1.1).
- Full details and formulas for each model are visible directly in the interactive data table and explanatory notes section inside the app.

---

## 🤝 Contributing

We welcome updates as new official benchmarks are published by Artificial Analysis, or as model pricing adjusts!
Please read our [Contributing Guide](CONTRIBUTING.md) to learn how to submit updates.

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).
