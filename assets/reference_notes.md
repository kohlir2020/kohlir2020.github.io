# Raunit Kohli — Consolidated Reference Notes

> **Purpose:** Single reference file for all raw content, research, links, and context about Raunit's
> work, projects, and career goals. Intended for use by AI agents and for personal reference when
> updating the resume, CV, or website. Last updated: April 2026.

---

## Table of Contents
1. [Career Goals & Target Roles](#career-goals--target-roles)
2. [Job Market Research (April 2026)](#job-market-research-april-2026)
3. [Graduate School Research](#graduate-school-research)
4. [Rocket Software — Detailed Content](#rocket-software--detailed-content)
5. [Chiba Lab (RUBI Lab) — Detailed Content](#chiba-lab-rubi-lab--detailed-content)
6. [Publications](#publications)
7. [Projects](#projects)
8. [Technical Stack & Skills](#technical-stack--skills)
9. [Website & Resume Architecture](#website--resume-architecture)
10. [Key Decisions & Distinctions](#key-decisions--distinctions)
11. [Links & References](#links--references)

---

## Career Goals & Target Roles

Raunit is targeting mid-career software engineering roles focused on:
- **Reinforcement Learning** (policy optimization, sim-to-real transfer)
- **Robotics Automation** (autonomous behavior, multi-agent systems, ROS2)
- **Agentic AI Applications** (LLM-powered agents, multi-agent workflows, tool use)

Also interested in **graduate school** (MS or PhD) in robotics/RL/AI at top programs.

---

## Job Market Research (April 2026)

### Industry Roles Researched
Searched for 2026 postings at companies aligned with Raunit's interests:

**Figure AI** — Robotics ML Engineer
- Keywords: PyTorch, RL, sim-to-real, policy optimization, C++, real-time systems
- Looking for: experience with physical robots, manipulation, locomotion

**Skild AI** — ML Engineer, Foundation Models for Robotics
- Keywords: large-scale RL training, simulation (MuJoCo/Isaac), multi-task learning
- Looking for: sim-to-real transfer, generalizable robot policies

**NVIDIA** — Robotics Research Scientist (Isaac Lab)
- Keywords: Isaac Sim/Gym, RL, sim-to-real, GPU-accelerated simulation, C++/CUDA
- Looking for: publications, simulation expertise, real robot deployment

**Apple** — ML Engineer, Robotics & Automation
- Keywords: RL, computer vision, motion planning, sensor fusion, ROS
- Looking for: production ML systems, real-world deployment experience

**General patterns across all postings:**
- PyTorch is universal for robotics/RL
- C++ is highly valued (real-time constraints)
- ROS/ROS2 is table stakes for robotics roles
- Sim-to-real transfer is a hot keyword (MuJoCo, Isaac, Habitat)
- Publications are a plus but not always required for industry
- Multi-agent systems / swarm robotics gaining interest
- LangChain/agentic AI is its own fast-growing category separate from robotics

### Gap Analysis (Profile vs. Market)
**Strengths already present:**
- PyTorch RL implementation with real robots (PiRat) — very rare and valuable
- ROS2 experience with actual hardware deployment
- C++ production CV work (300% speed improvement)
- Multi-agent experimental data (2500+ sessions)
- Published research (3 papers, 2nd author on ICDL)
- Agentic AI production work (LangChain, DSPy, ReAct agents)
- Leadership (1800+ engineers trained, AI Center of Excellence)

**Gaps identified and addressed:**
- ✅ "Reinforcement Learning" keyword was missing from skills → added to Domains
- ✅ Libraries line was commented out in LaTeX → restored with DSPy, MLflow added
- ✅ ROS2 not explicit (was just "ROS") → corrected to ROS2
- ✅ MuJoCo/sim-to-real language missing → added via Regulation project
- ✅ No Docker/deployment keywords → added via EVA product
- ⚠️ No public GitHub repos (most code NDA'd/under grants) — user may create 1-2
- ⚠️ Google Scholar profile not publicly findable — user says they're on it
- ⚠️ PiRat RL project page on website still has placeholder text

---

## Graduate School Research

### Programs Researched
- **CMU Robotics Institute** (MS/PhD): Strong RL + robotics focus. Values publications, real robot experience, C++ systems work.
- **Stanford CS** (MS/PhD AI track): Values breadth across ML + systems. Publications important for PhD.
- **MIT CSAIL** (Robotics): Hardware + software integration valued. Real-world deployment experience a plus.
- **UC Berkeley BAIR** (PhD): Strong RL tradition (Abbeel, Levine). Sim-to-real transfer research.

### What Grad Schools Want (CV Optimization)
- Publications are critical (Raunit has 3, including 2nd author ICDL 2025)
- Research experience duration matters (Raunit: 4+ years)
- Recommendation letters from PIs (Chiba Lab relationship is strong)
- Technical depth > breadth on CV
- Teaching experience is a plus (TA + AI enablement + VEX coaching)
- GPA threshold usually 3.5+ (Raunit: 3.91 major GPA — excellent)

---

## Rocket Software — Detailed Content

### Rocket EVA (AI Platform)
- **Product page:** https://www.rocketsoftware.com/en-us/products/eva (was 403'd when checked April 2026)
- Raunit owns multiple core features:
  - RESTful API design
  - End-to-end OIDC Authorization pipeline
  - Live telemetry/streaming pipelines
  - Asynchronous tool execution pipeline
  - Fixed at least half the coding bugs for first product release
  - Structured Docker deployment pipeline
  - Owning integration with Rocket teams' products into EVA
  - Worked with ID teams for internal and public-facing documentation
- Most aggressively promoted and marketed company-wide tool

### SAS-to-Python Code Translation
- Specialized team project using multiple LLM-optimization techniques
- Built large-scale datasets and model evaluation pipelines
- Used ReAct agent (Reasoning+Action agent) via LangChain
- Collaborated on Agentic Context Engineering (ACE) optimizer
  - ACE paper: https://arxiv.org/abs/2510.04618 (ICLR 2026)
  - **IMPORTANT: Raunit is NOT an author on this paper** — he collaborated on/used the framework
- Created multi-agent workflows for: planning, architecture design, test generation, custom live code execution, refinement loops
- Integrated with MLflow for logging/evaluation

### SmartChat (RAG System)
- **Brochure:** https://www.rocketsoftware.com/sites/default/files/resource_files/smart-chat-brochure.pdf
- Raunit built: SQL generation/execution pipeline, Citations feature (multi-Gaussian clustering, 80% improvement), Feedback API, Reranking feature, AWS CloudWatch logging system
- NL-to-SQL retrieval agent with regex-based syntax validation
- Fine-tuned transformer-based sentence embedding models with custom tokenizers

### AI Enablement & Teaching
- Created entire AI foundations and enablement lecture series for NextGen program
  - **NextGen Academy:** https://www.rocketsoftware.com/en-us/nextgen-academy
- Delivered AI foundations lecture series at global Rocket offices, achieving 100% content application rate
- 100% content application rate (every audience member applied tools/techniques to daily work)
- Workshops solve real-world problems on existing Rocket engineering teams
- Leading collaboration with 3rd party vendor for company-wide AI enablement (1800+ engineers)
- Week-long lecture series covering: GenAI foundations, LLM conceptual understanding, prompt engineering, model tuning, workflow building, AI-assisted coding

### Smart Scrum Master (Hackathon)
- 2025 Rocket.Build Hackathon — **Won "Most Innovative" award** (1 of 6 winners from 650+ projects globally)
- LLM-powered Agile assistant optimizing Jira workflows
- Securely updates/creates/searches/summarizes Jira tickets based on user queries or Teams meeting content
- Uses reasoning agent for intelligent Jira board organization
- Exposed as MCP Server — can be hosted by other chatbots and IDEs
- Project served as a foundation for AI-focused workflow optimizations and developer enablement trainings
- Acted as basis for subsequent AI-focused optimizations and developer enablement trainings

### Other Rocket Details
- AI Center of Excellence — working with the CoE to bring advanced AI tooling to expert engineers (NOT a founding member; does NOT collaborate with DSPy creators — DSPy is just a library used)
- Main languages/libraries: Python, DSPy, LangChain, PyTorch, HuggingFace
- MultiValue Experience Unit Test Coverage project (earlier role): launched foundational unit test framework with OOP mocking, 30% line coverage (3x OKR goal)

---

## Chiba Lab (RUBI Lab) — Detailed Content

### Lab Info
- Full name: Robotics Using Bayesian Inference Lab, UC San Diego
- PI: Professor Andrea A. Chiba
- Lab website: https://www.chiba-lab.org/ (unfinished as of April 2026)
- Raunit's tenure: Staff ML Research Engineer (01/2021–09/2024), ML Research Consultant (09/2024–present)

### PiRat Robot System (Technical Deep-Dive)
From content.md's detailed tech stack description:

**The Robot:**
- Rat-sized mobile robot for studying social behavior in rats
- Electronics: three stacked circuit boards (Raspberry Pi Zero footprint)
  - Top: Raspberry Pi Zero (Raspbian, Wi-Fi via wireless card)
  - Middle: Distribution board with STM32 F042 microcontroller (USB to Pi Zero, PWM to encoders, USART to driver)
  - Bottom: Custom two-gimbal motor driver based on Martinez Gimbal board
- Weight: 0.24kg, top speed: 1.1m/s, top angular velocity: 4.7m/s
- Reference: "PiRat: An autonomous framework for studying social behaviour in rats and robots." IROS 2018.

**Behavior Controller (GUI):**
- External GUI built in Python with Kivy
- Captures live global top-down positions of all agents in circular arena
- Calculates target linear/angular velocity based on PiRat position/orientation
- Multiple finite-state machine inspired autonomous behaviors
- Homebase detection: convolution sliding kernel over frequency distribution of positions
- Target position: next pose on trajectory that intersects or circumvents homebase
- Updates Kivy GUI + sends velocity commands via ROS2

**Tracking System:**
- Multi-threaded Python script
- Live-inference pose estimation using SLEAP (Social LEAP Estimates Animal Poses)
- Pipeline: load pre-trained neural networks → capture RGB frames → inference → dynamic memory array → visualization overlay
- Poses streamed to behavior controller in real-time

**NeuroPos Composable Pipeline:**
- Location: `/Users/raunit/Desktop/ChibaLab/NeuroPosHb/`
- Modular processing steps (discovered from directory):
  - HomebaseDetection (convolution kernel)
  - SpectralFeatures
  - SpatialAnalysis
  - Signal processing modules
- Integrated pose-estimation + neural signal data analysis
- Used across 2500+ experimental sessions

**PiRat Software Stack:**
- Location: `/Users/raunit/Desktop/ChibaLab/pirat/`
- Multi-threaded SLEAP + Kivy GUI + ROS behavior control
- ROS2 (NOT ROS1)

### RL Regulation Framework
- MuJoCo simulation environment
- Uses Google DeepMind tools
- Multiple policy optimization algorithms (PPO, SAC)
- Models exploration-regulation dynamics in autonomous robotic behavior
- Bio-influenced: mimicking rat grooming behaviors for positive exploration-regulation effects
- Ongoing/confidential — keep descriptions general
- Designed for sim-to-real transfer to physical PiRat robot

### AI Classroom Project
- **Sponsor:** (user clarified: project has nothing to do with HEDC — removed from all docs)
- Multi-million dollar project
- Raunit was founding engineer hired
- Built initial pilot system for multimodal live synced secure data streaming/recording in Pre-K classroom
- Main point of contact for technical specifications
- Architecture based on PTPv2 (Precision Time Protocol v2)
- Components confirmed by user:
  - High-precision Basler cameras
  - Custom Arduino firmware for OpenBCI Emotibits (biophysical signal detection)
  - Lab Streaming Layer (LSL)
  - PTPv2 synchronization
- Exhaustive knowledge transfer sessions with new hires
- Note: "Dante networking", "on-prem quartz crystal grandmaster clock", "neuromorphic sensors", and "wearable physiological monitors" were found during directory exploration but NOT confirmed by user — do not include on resume without confirmation
- Can be categorized under either Staff Researcher or Consultant role

### Research Team Management
- Hired and trained undergraduate research assistants (RAs)
- RAs learned system operation and experiment execution
- Established knowledge transfer documentation for long-term project continuity

### Publications
See [Publications](#publications) section below.

---

## Publications

1. **ICDL 2025** (2nd author): I. Jackson, **R. Kohli**, E. Leonardis, V. R. de Sa, S. Fei, L. Quinn, Y. Lou, A. A. Chiba. "Explore-Exploit Behaviors During Rat-Robot Interactions Optimize Social and Spatial Security." *IEEE International Conference on Development and Learning*, 2025.
   - IEEE: https://ieeexplore.ieee.org/document/11204421

2. **Frontiers in Psychology 2022**: E. Leonardis, A. Bhaskara, S. Fei, **R. Kohli**, A. A. Chiba. "Interactive neurorobotics: Behavioral and neural dynamics of agent interactions." *Frontiers in Psychology*, Sec. Cognitive Science, Vol. 13, 2022.
   - DOI: https://doi.org/10.3389/fpsyg.2022.897603

3. **BCI 2025** (Abstract): I. Jackson, **R. Kohli**, E. Leonardis, S. Fei, L. Quinn, V. R. de Sa, A. A. Chiba. "Robotic Exploratory Control Via Subcortical Oscillations." *11th International Brain-Computer Interface Meeting*, 2025.
   - PDF: https://openlib.tugraz.at/download.php?id=686289f5ddb80&location=browse

---

## Projects

### VLM-Guided Hierarchical RL in Habitat-Lab (WPI, 2024)
- Hierarchical PPO/SAC for Fetch robot
- Vision-Language Model high-level planner
- Autonomous navigation and manipulation from language instructions
- Reward shaping and policy optimization across dual-layer hierarchy

### Smart Scrum Master (Rocket.Build 2025)
- See Rocket Software section above

### Aspera Workflows Automated Test Suite (IBM, 2023)
- Ruby automation of API endpoint testing for IBM Aspera on Cloud Workflows
- 780+ automated regression tests covering all endpoints
- Identified 15+ critical production bugs
- Full development cycle for API Endpoint Test Controller
- Contributed to global watsonx AI hackathon

### VEX Robotics Autonomous Systems Coaching (GHS)
- Mentoring competitive VEX Robotics team
- Autonomous path planning: PID control, cubic spline trajectory generation, odometry-based localization, sensor fusion
- Curriculum covers control theory fundamentals, directly maps to ROS-based architectures

### MultiValue Experience Unit Test Coverage (Rocket)
- Foundational unit test framework with OOP mocking and line coverage
- 30% line coverage (3x initial OKR goal)
- Identified multiple redundant dependencies

---

## Technical Stack & Skills

### Languages
Python, C++, Ruby, Java, SQL, Bash

### Libraries & Frameworks
PyTorch, DSPy, LangChain, HuggingFace, MLflow, Pandas, NumPy, Scikit-learn, Kivy, OpenBCI

### Domains
Reinforcement Learning, Multi-Agent Systems, Agentic AI, NLP, Computer Vision, Sim-to-Real Transfer, Policy Optimization (PPO/SAC), Signal Processing, Pose Estimation, Neurorobotics, Embedded Systems

### Tools & Platforms
ROS2, MuJoCo, SLEAP, Habitat-Lab, Docker, AWS (CloudWatch), Kubernetes, Git/GitHub, Atlassian Suite (Jira, Confluence), Arduino, PTPv2, Lab Streaming Layer (LSL)

### Coursework
Deep Learning for NLP, Neural Networks, Data Modeling, Advanced Topics in LLMs, Supervised & Unsupervised ML, Data Structures & Algorithms, Markov Decision Processes, Reinforcement Learning (WPI)

---

## Website & Resume Architecture

### Website
- Jekyll site on GitHub Pages at raunitkohli.com (CNAME file present)
- Layout: `_layouts/default.html` → includes `header.html` + `footer.html`
- Config: `_config.yml` with nav items (Home, Industry, Research, Extracurricular, Resume)
- Pages: index.html, work.html, research.html, extracurricular.html, resume.html
- Resume page has dual download buttons (Industry Resume + Academic CV) with PDF preview iframes

### Resume Files
- `assets/rk_resume.tex` — 1-page industry resume (LaTeX source)
- `assets/rk_cv.tex` — Multi-page academic CV (LaTeX source)
- `assets/rk_resume.pdf` — Compiled industry resume PDF
- `assets/rk_cv.pdf` — Compiled academic CV PDF (needs to be generated)
- `assets/Raunit_Resume_Feb_25.pdf` — Older Feb 2025 version (kept for reference)

### LaTeX Template Details
- Based on sb2nov/resume template
- Custom commands: `\resumeSubheading`, `\resumeItem`, `\resumeItemListStart/End`, `\resumeSubHeadingListStart/End`
- RUBI Lab section uses manual `\vspace{-2pt}\item` + `\begin{tabular*}` blocks (two sub-roles under one org)
- Both fontawesome (v4) and fontawesome5 loaded; v4 takes precedence
- Industry resume: aggressive margins (oddsidemargin -0.6in, topmargin -0.7in), negative vspace (-14pt to -20pt)
- CV: slightly relaxed margins (oddsidemargin -0.5in, topmargin -0.5in)

### Compilation
```bash
cd assets
pdflatex rk_resume.tex   # Industry resume
pdflatex rk_cv.tex        # Academic CV
rm -f *.aux *.log *.out   # Clean artifacts
```
Requires LaTeX distribution (macOS: `brew install --cask basictex`)

---

## Key Decisions & Distinctions

- **ACE framework (arxiv:2510.04618):** Raunit collaborated on/used the ACE framework but is NOT an author. Resume says "collaborating on ACE optimization framework", not "co-authored."
- **AI Center of Excellence:** Raunit works WITH the CoE. He is NOT a "founding member" and did NOT "collaborate with DSPy library creators." DSPy is simply a library he uses.
- **AI enablement numbers:** User's own lectures achieved 100% application rate. The 1800+ engineers number is about a vendor collaboration the user coordinates, NOT the user's direct training audience.
- **Country names:** User said "global Rocket locations" but did NOT list specific countries. Do not fabricate country lists.
- **ICDL 2025:** Raunit IS 2nd author — strong position.
- **Google Scholar:** Raunit claims to be listed but no public profile URL was found. Kept as commented-out placeholder in CV LaTeX.
- **RL Regulation project:** Ongoing/confidential — descriptions kept general (MuJoCo, multiple policy algorithms, exploration-regulation dynamics).
- **Code availability:** Most code is NDA'd or under active research grants. User may create 1-2 public repos but can't share most work.
- **PiRat uses ROS2** (NOT ROS1 as might be assumed from older papers).
- **Two resume versions:** 1-page industry resume focuses on high-impact bullets and keywords; multi-page CV expands everything for academic audiences.
- **IBM internship:** Removed as a work experience section on industry resume; Aspera test suite is a project there. Full IBM section retained on CV.
- **AI Classroom placement:** Listed under Research Consultant role (current) on industry resume; could fit under either Staff or Consultant role per user.
- **AI enablement numbers:** User's own lectures achieved 100% content application rate. The 1800+ engineers number is about a vendor collaboration program the user is coordinating, NOT the user's direct training audience. These must be described separately.
- **Country names:** User said "global Rocket locations" — specific countries (US, India, UK, Czech Republic, China) were NOT provided by user and should not be listed.

---

## Links & References

### Raunit's Properties
- Website: https://www.raunitkohli.com/
- GitHub: https://github.com/kohlir2020
- LinkedIn: https://linkedin.com/in/raunit-kohli/
- Email: raunitkohli@gmail.com
- Phone: 774-262-9233

### Publications
- ICDL 2025: https://ieeexplore.ieee.org/document/11204421
- Frontiers 2022: https://doi.org/10.3389/fpsyg.2022.897603
- BCI 2025 Abstract: https://openlib.tugraz.at/download.php?id=686289f5ddb80&location=browse

### Rocket Software
- EVA Product: https://www.rocketsoftware.com/en-us/products/eva
- SmartChat Brochure: https://www.rocketsoftware.com/sites/default/files/resource_files/smart-chat-brochure.pdf
- NextGen Academy: https://www.rocketsoftware.com/en-us/nextgen-academy
- ACE Paper (ICLR 2026, NOT authored): https://arxiv.org/abs/2510.04618

### Research
- Chiba Lab Website: https://www.chiba-lab.org/ (unfinished)
- PiRat IROS 2018 Paper: https://doi.org/10.1109/iros.2018.8594060

### Local Directories (for code context)
- NeuroPos Pipeline: `/Users/raunit/Desktop/ChibaLab/NeuroPosHb/`
- PiRat System: `/Users/raunit/Desktop/ChibaLab/pirat/`

### Job Posting Companies Researched
- Figure AI (robotics ML)
- Skild AI (foundation models for robotics)
- NVIDIA Isaac Lab (robotics research)
- Apple (robotics & automation ML)

### Graduate Programs Researched
- CMU Robotics Institute
- Stanford CS (AI track)
- MIT CSAIL
- UC Berkeley BAIR

---

## Known Website Issues (Future Work)
- PiRat RL project on research.html still has placeholder text ("[Summary to be added]")
- VEX Robotics on extracurricular.html may need expansion
- index.html has "Please hire me!" text that could be more professional
- Google Scholar link needs to be added once profile URL is confirmed
