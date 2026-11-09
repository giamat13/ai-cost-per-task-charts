# Contributing Guidelines

Thank you for your interest in contributing to **AI Cost Per Task Charts**!

We welcome contributions of all kinds: adding new benchmark measurements, refining estimation models, reporting inaccuracies, improving visual charts, or enhancing user experience.

---

## How to Contribute

### 1. Adding or Updating AI Model Data
The model dataset is maintained in `index.html` inside the `MODELS` array.

Each model entry follows this structure:
```javascript
{
  model: 'Model Name',
  color: '#hexcolor',
  def: true, // true to show by default on chart load, false otherwise
  points: [
    {
      effort: 'low',      // 'low' | 'medium' | 'high' | 'xhigh' | 'max'
      cost: 0.9800,       // Average cost per task in USD
      score: 35.00,       // Benchmark intelligence index score
      measured: true,     // true if directly measured by Artificial Analysis, false if estimated
      kind: 'measured',   // 'measured' | 'estimated' | 'measured cost, estimated score'
      src: 'v5 (AA)'      // Citation or estimation method
    },
    // ...
  ]
}
```

When submitting new data:
- **Prioritize verified measurements**: Always include reference links or citations in PR descriptions.
- **Mark estimated data explicitly**: If a data point is estimated or extrapolated, set `measured: false` and document the exact methodology/ratios in the `src` property and notes section.

### 2. Submitting Pull Requests
1. **Fork** the repository on GitHub.
2. **Create a branch** for your feature or data update:
   ```bash
   git checkout -b update/model-name-benchmark
   ```
3. **Commit your changes** with clear, descriptive commit messages:
   ```bash
   git commit -m "Add measured v5 benchmark points for Model X"
   ```
4. **Push** your branch:
   ```bash
   git push origin update/model-name-benchmark
   ```
5. **Open a Pull Request** describing what changed, data sources, and any calculations used.

---

## Reporting Issues & Feature Requests
- Check the [Issues](../../issues) tab to see if the issue or request is already being discussed.
- If not, open a new issue detailing:
  - Description of the issue or discrepancy.
  - Links to official source benchmarks or pricing changes.
  - Expected vs. actual behavior.

---

## Community Guidelines
Please be respectful and constructive in all discussions, pull requests, and issues.
