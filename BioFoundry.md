# BioFoundry — From Sequence to Solution

BioFoundry is an open-source computational biology platform for primer design, genome-aware validation, and CRISPR-integrated experimental planning. It is designed to streamline the workflow from raw DNA sequence input to validated experimental output using a modular, extensible, and AI-ready architecture.

---

## 🚀 Mission

To empower researchers, educators, and developers with a unified platform that connects:
- Primer design
- Genome validation
- CRISPR experiment planning
- AI-assisted biological reasoning

From sequence to solution — and eventually from idea to experiment.

---

## 🧬 Core Features

### 🟢 Primer Design Engine
- Forward and reverse primer generation
- Primer pair optimization
- Amplicon size control
- GC content balancing
- Melting temperature (Tm) calculation
- Primer ranking system
- Multi-candidate primer generation
- Batch primer design support

---

### 🔬 Sequence Handling
- FASTA file input support
- Raw sequence input support
- Multi-sequence batch processing
- Region and gene targeting tools
- Sequence validation and sanitization

---

### ⚙️ Scoring & Stability Analysis
- GC content scoring
- Tm optimization scoring
- Hairpin structure detection
- Self-dimer detection
- Cross-dimer detection
- Primer specificity scoring

---

### 🧬 Genome Validation Layer
- Multi-genome support
- Genome indexing system
- BLAST integration for off-target detection
- Bowtie integration support
- SNP-aware primer filtering
- Repeat-region detection
- Genome-wide binding risk analysis

---

### 🔍 Off-Target Detection System
- Primer genome-wide mapping
- Multi-hit detection warnings
- Off-target scoring system
- Risk classification (low / medium / high)
- Cross-reactivity detection with genomic regions

---

### 🔵 CRISPR Integration Module
- gRNA input and mapping support
- Primer + gRNA co-design system
- CRISPR cut-site mapping
- Knockout validation primer design
- Knock-in validation primer design
- HDR junction primer design
- Base editing validation support
- Prime editing validation support
- PAM region awareness layer
- Off-target overlap detection (primer vs gRNA)

---

### 🟣 AI Intelligence Layer
- AI-assisted primer ranking suggestions
- Experimental goal interpretation
- Explanation of primer selection decisions
- Failure prediction heuristics
- CRISPR experiment strategy suggestions
- qPCR / PCR / NGS workflow recommendations
- Context-aware scoring adjustments

---

### 📊 Visualization Layer
- Primer binding visualization
- Amplicon mapping visualization
- Genome hit visualization
- Hairpin and dimer structure visualization
- Off-target mapping display
- Sequence region highlighting

---

### ⚙️ API & CLI System
- REST API (FastAPI-based architecture)
- CLI primer design tool
- Batch processing support
- JSON output schema
- Pipeline-friendly execution mode

---

### 📁 Lab Workflow System
- Experiment project tracking
- Primer version history
- Rollback support
- Structured lab organization system
- Multi-experiment management

---

### 📤 Export System
- CSV export
- JSON export
- Benchling-compatible formats
- SnapGene-compatible formats
- Markdown lab notebook export

---

### 🌍 Community & Open Source Layer
- AGPL-3.0+ licensed ecosystem
- GitLab-based development workflow
- Issue-driven contribution system
- Merge request validation pipeline
- Plugin architecture support
- Community scoring extensions
- Genome adapter plugins
- Validation strategy plugins
- Optional shared primer library
- Reproducible experiment tracking

---

### 🚀 Advanced / Future Features
- AI autonomous experiment planner
- Natural language experiment generation
- CRISPR simulation engine (in-silico edits)
- Reinforcement learning primer optimization
- Cross-species primer transfer learning
- Collaborative cloud lab environments
- Real-time multi-user design sessions
- Wet-lab automation integration APIs

---

## 🧠 Project Vision

BioFoundry aims to become a full-stack computational biology platform that connects:

1. Sequence input  
2. Primer design  
3. Genome validation  
4. CRISPR-aware experiment planning  
5. AI-assisted biological reasoning  
6. Community-driven scientific expansion  

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/biofoundry/](https://roxanneardary.com/biofoundry/)

---

## 🧾 License & Notice Requirements

BioFoundry is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- BioFoundry specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.  

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
