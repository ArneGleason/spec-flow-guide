
# Spec-Flow

**Requirements-First, AI-Accelerated Product Development**

Spec-Flow is a lightweight framework and reference implementation for building modern applications by treating written specifications as the single source of truth and letting AI tools generate, test, and continually regenerate the codebase.  
This repository hosts the living handbook, sample artefacts, and automation scripts you need to adopt the process in your own teams.

---

## Why Spec-Flow?

* **Shorter lead times** – Well-formed stories flow straight into AI code generation and automated test creation.  
* **Lower technical debt** – Regeneration sprints keep the codebase fresh and consistent instead of patching over legacy layers.  
* **Total traceability** – Every line of code maps back to a specific requirement and architectural decision.  
* **Future-proofing** – As AI capabilities improve, rerunning the same spec yields better, leaner code without manual rewrites.  

---

## Repository Structure

```

.
├── README.md              ← This file
├── LICENSE                ← Code licence (Apache-2.0 by default)
├── LICENSE-DOCS           ← Docs licence (CC-BY-4.0)
├── docs/
│   ├── vision.md          ← One-page Spec-Flow vision
│   └── handbook.md        ← Detailed process handbook
├── specs/
│   ├── vision/            ← Vision briefs for sample projects
│   ├── architecture/      ← Architecture notes & diagrams
│   └── charter/           ← Product charters and KPI sets
├── backlog/
│   ├── epics/             ← Epics & capabilities
│   └── stories/           ← User stories with acceptance criteria
├── prompts/               ← Re-usable system prompts & few-shot examples
├── src/                   ← Example generated code
├── tests/                 ← Auto-generated test suites
└── regen/                 ← Scripts for full regeneration cycles

````

---

## Quick Start

1. **Clone the repo**

   ```bash
   git clone https://github.com/<your-org>/spec-flow-handbook.git
   cd spec-flow-handbook
````

2. **Read the vision**

   Start with `docs/vision.md` to understand the goals and guiding principles.

3. **Run the demo regeneration script**

   ```bash
   ./regen/run-demo.sh
   ```

   This script pins a local AI model, ingests the sample stories in `backlog/`, and produces a fresh build in `src/`.

4. **Explore the traceability report**

   After the script completes, open `regen/output/traceability.html` in your browser to see how code lines link back to requirements.

---

## Contributing

Pull requests are welcome for:

* Improvements to the handbook or vision
* Better prompt engineering examples
* Additional regeneration utilities or CI integrations
* Real-world case studies using Spec-Flow

Before contributing, please read `CONTRIBUTING.md` for coding standards and contribution workflow.

---

## License

* **Code and scripts:** Apache License 2.0 (see `LICENSE`)
* **Documentation and diagrams:** Creative Commons Attribution 4.0 (see `LICENSE-DOCS`)

You may reuse either or both licences when adopting Spec-Flow materials.

---

## Maintainers

Spec-Flow is stewarded by the community. Open an issue or discussion thread if you’d like to become an active maintainer or propose significant changes.

---

*Write the spec. Let AI flow.*

```

Feel free to tweak directory names, licensing details, or quick-start commands to match your actual repo setup.
```
