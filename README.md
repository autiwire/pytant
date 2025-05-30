# Pytant – Minimal AI Patent Forge

**Author:** Rouven Raudzus  
**Company:** AutiWire GmbH  
**Date:** 2025-05-30  
**License:** Apache 2.0

---

## 🧾 Title of the Invention

**Pytant – Minimal Repository-Based System for AI-Supported Patentable Idea Development**

---

## 🧠 Technical Field

This invention relates to the field of intellectual property (IP) systems, specifically to lightweight, repository-based structures for managing, documenting, and optionally protecting AI-supported inventions.

---

## 🔍 Background of the Invention

Current AI-based patent tools focus on claim writing, prior art comparison, and text optimization. These include tools such as DeepIP, AutoPatent, and PatentGPT. However, these existing systems generally involve complex interfaces and emphasize automation of later-stage patent processes, lacking support for the initial creative ideation phase. They typically do not document the idea generation workflow itself, nor do they integrate version control effectively to ensure auditability and traceability. Moreover, they often treat AI purely as an automation tool rather than as an active co-agent in collaboration with humans.

Thus, there exists a clear need for a minimal, lightweight, human-first approach that leverages AI support to systematically document, structure, and optionally protect early-stage, novel ideas without relying on complex legal tools or specialized software.

---

## 🔎 Summary of the Invention

This invention provides a repository structure where AI models — under user instruction — generate, refine, and export invention drafts. The system uses markdown- and folder-based workflows, version control (e.g., Git), and a simple instruction file (`INSTRUCTIONS.md`) to:

* Structure the invention process from ideation to export
* Enable AI code editors (e.g., Cursor, Copilot) to participate in the ideation
* Record authoring and review steps for legal audit
* Generate defensible claims and outputs ready for IP registration or publication

---

## 🌐 Sample Implementation

A public implementation of this system is available at:

[https://github.com/autiwire/pytant](https://github.com/autiwire/pytant)

This repository serves both as a reference implementation and a live demonstration of the system in action.

## 📐 Detailed Description of the Invention

The repository contains the following core elements:

```
pytant/
├── INSTRUCTIONS.md         # Central protocol for AI-human interaction
├── ideas/                  # Early-stage idea files (YAML, MD)
├── claims/                 # Drafted patent-like texts
├── outputs/                # Export bundles (e.g. disclosure packages)
└── README.md               # This file — doubling as specification
```

### AI Interaction

The system assumes a human-in-the-loop setup where AI proposes structures, claims, and summaries based on guidance in `INSTRUCTIONS.md`. Every file generated is recorded in a timestamped Git commit. Personas and authorship information can be layered using optional metadata.

### Export

Ideas and claims can be exported as `.zip` or `.md` via scripting (e.g. Python), and automatically published to defensive archives (GitHub, ArXiv, Zenodo).

---

## 📄 Example Claims (non-limiting)

1. A repository-based system for generating, recording, and protecting AI-assisted patentable ideas via instruction-guided human-AI interaction.
2. The system of claim 1, wherein each output file is timestamped and version-controlled for traceability.
3. The system of claim 1, wherein no structured schema, manifest, or legal tooling is required.
4. The system of claim 1, wherein a single README file serves simultaneously as project overview and invention specification.
5. The system of claim 1, wherein an instruction file defines interaction logic between human and AI editor.

---

## License Notice

This system is licensed under the Apache License 2.0. This application serves as a public disclosure and may also serve as a basis for a provisional patent claim. Usage of the system is permitted under the terms of the Apache 2.0 License, with no further restrictions imposed. Any commercial use, redistribution, or sublicensing beyond personal research or evaluation purposes requires separate permission or licensing from AutiWire GmbH.

---

## 📜 Terms of Use

By using this system, users agree to the [Terms of Use](./TERMS.md).  
These terms include clauses on intellectual property (IP) ownership, participation rights, and commercial usage.  
Use of the system without agreement to these terms is prohibited beyond non-commercial evaluation or research purposes.

---

## 🛡️ Legal Note

This README serves as a specification and public disclosure of the invention, as part of a provisional patent filing. It is protected under the Apache 2.0 license and structured for possible patent submission. This disclosure is intended to establish prior art and serves as a defensive publication, preventing others from patenting similar inventions. It is also intended to be recognized as prior art in the event that similar concepts are submitted for patenting, thereby ensuring that this invention remains free from patent infringement. Any contributions made by external parties to this repository are governed by the terms of the Apache 2.0 license and the Terms of Use outlined in [TERMS.md](./TERMS.md).

The Apache 2.0 License and the accompanying Terms of Use govern the use and participation in this project, ensuring clarity on intellectual property ownership, commercial licensing, and contribution rights.

This tool does not constitute legal advice or patent consultation. It supports technical documentation and ideation only. For legal assessments or formal patent filing, always consult a qualified attorney.

If any prior art overlaps with this concept, please contact `raudzus@autiwire.de`.

---

## 📬 Contact

**📧 [raudzus@autiwire.de](mailto:raudzus@autiwire.de)**  
For collaborations, legal use, or audit reference.

---

**This README is the invention. This repo is the patent forge.**  
**Minimal structure. Maximum effect.**
