# Copilot Instructions — raunitkohli.com

## Project Overview
Personal website and resume/CV for **Raunit Kohli**, an ML Software Engineer at Rocket Software and Research Consultant at UCSD's Chiba Lab. The site is a Jekyll static site deployed on GitHub Pages at [raunitkohli.com](https://www.raunitkohli.com). The repo also contains LaTeX source for a 1-page industry resume and a multi-page academic CV.

**Target roles:** Mid-career software engineering in reinforcement learning, robotics automation, and agentic AI applications, plus graduate school (CMU, Stanford, MIT, Berkeley).

## File Structure

### Website (Jekyll)
- `index.html` — Homepage with summary, LLM/RL project boxes, social links
- `work.html` — Industry projects (EVA™, SAS Translation, AI Enablement, Smart Scrum, SmartChat™, Aspera, MultiValue)
- `research.html` — Publications (ICDL 2025, Frontiers 2022, BCI 2025) and research projects (PiRat Homebase, RL Regulation, AI Classroom)
- `extracurricular.html` — VEX Robotics coaching, Phi Sigma Pi, TA, Philosophy
- `resume.html` — Dual download buttons + PDF preview iframes for resume and CV
- `_layouts/default.html` — Main layout; includes `_includes/header.html` and `_includes/footer.html`
- `_config.yml` — Site config with nav links
- `style.css` — All custom styles

### Resume & CV (LaTeX)
- `assets/rk_resume.tex` → `assets/rk_resume.pdf` (1-page industry resume)
- `assets/rk_cv.tex` → `assets/rk_cv.pdf` (multi-page academic CV)
- Template: sb2nov/resume with custom commands (`\resumeSubheading`, `\resumeItem`, etc.)
- **RUBI Lab section** uses manual `\vspace{-2pt}\item` + `\begin{tabular*}` blocks (NOT `\resumeSubheading`) because it has two sub-roles (Consultant + Staff) under one organization heading
- Both `fontawesome` (v4) and `fontawesome5` are loaded; v4 takes precedence
- **Compile:** `cd assets && pdflatex rk_resume.tex` / `pdflatex rk_cv.tex`

### Reference Documents
- `assets/content_provenance.md` — Line-by-line audit of every resume/CV bullet with source attribution. Documents hallucinations that were caught and corrected.
- `assets/reference_notes.md` — Consolidated research notes, raw content from all sources, technical decisions, and corrections log.
- `assets/old/` — Archived originals: `Raunit_Resume_2024.pdf`, `Raunit_Resume_Feb_25.pdf`, `content_old.md`, `Assorted_notes_old`. Do NOT delete these.

## Critical Content Rules

### NEVER Hallucinate
Previous AI sessions fabricated content including fake publication authors, countries visited, collaborator relationships, and role titles. Every factual claim MUST trace to one of these sources:
- The user's own statements or edits
- `assets/old/Assorted_notes_old` (user's raw notes)
- `assets/old/Raunit_Resume_2024.pdf` or `assets/old/Raunit_Resume_Feb_25.pdf` (older resume versions)
- Published papers (verified via DOI/IEEE links)
- `assets/content_provenance.md` (audit trail)

### Specific Rules (from user corrections)
- **AI Center of Excellence:** Raunit "works with" the CoE. He is NOT a "founding member" and does NOT collaborate with DSPy library creators. DSPy is simply a library he uses.
- **Country names:** User said "global offices." Do NOT list specific countries.
- **AI Classroom:** Has NOTHING to do with HEDC. Do not add "HEDC-funded."
- **TensorFlow:** User does NOT know TensorFlow. Do not add it anywhere.
- **Smart Scrum Master:** "Served as a foundation for AI-focused workflow optimizations." Was NOT "selected for productionization."
- **ACE paper** (arxiv:2510.04618): User collaborated on/used the framework but is NOT an author.
- **PiRat uses ROS2** (not ROS1).
- **Sim-to-real IS applicable:** PiRat homebase behavioral routines are simulated then transferred to real robot velocity commands.
- **GHS = Grafton High School, Massachusetts** (not "Groves").
- **Phi Sigma Pi 2022 DC Convention** is confirmed (video at vimeo.com/873331411).
- **Never combine separate projects** into one bullet or mix descriptions between projects.
- **Resume bullets should be professional, well-worded, high-impact, skill-based, and naturally written.** The goal is to showcase skills over being faithful to the actual product.

### Publication Authors (verified)
1. **ICDL 2025:** I. Jackson, R. Kohli, E. Leonardis, V. R. de Sa, S. Fei, L. Quinn, Y. Lou, A. A. Chiba
2. **Frontiers 2022:** E. J. Leonardis, L. Breston, R. Lucero-Moore, L. Sena, R. Kohli, L. Schuster, L. Barton-Gluzman, L. K. Quinn, J. Wiles, A. A. Chiba
3. **BCI 2025:** I. Jackson, R. Kohli, R. Lucero-Moore, Y. Lou, L. K. Quinn, L. Breston, J. Wiles, A. A. Chiba, E. Leonardis

### Verified External Links
- EVA: https://www.rocketsoftware.com/en-us/products/eva
- SmartChat: https://www.rocketsoftware.com/sites/default/files/resource_files/smart-chat-brochure.pdf
- ICDL: https://ieeexplore.ieee.org/document/11204421
- Frontiers: https://doi.org/10.3389/fpsyg.2022.897603
- BCI: https://openlib.tugraz.at/download.php?id=686289f5ddb80&location=browse
- Google Scholar: https://scholar.google.com/citations?user=abZZ14QAAAAJ
- PSP Video: https://vimeo.com/873331411
- TA Podcast: https://podcast.ucsd.edu/watch/fa23/cogs108_a05

## Resume vs CV Strategy
- **Industry Resume** (1 page): Aggressive margins, curated bullets for RL/robotics/agentic AI roles. User actively trims this themselves.
- **Academic CV** (multi-page): Expanded version with all bullets, publications, coursework, teaching, leadership. Keep everything from the resume PLUS additional detail.
- When syncing changes: Update CV wording to match resume edits, but NEVER remove CV-only bullets.

## Known Minor CV-Website Gaps (intentional)
These CV items are intentionally NOT on the website (too granular for a web page):
- Fine-tuning embeddings, feedback API, AWS CloudWatch, customer collaboration bullets
- IBM watsonx hackathon, Rocket intern training series bullets
- NeuroPos pipeline, Hermite Splines/Pure Pursuit (supporting research details)
- Coursework section (Deep Learning for NLP, Neural Networks, etc.)
- Data visualization, statistical pipelines bullets

## User's Verified Skills
**Languages:** Python, C++, Ruby, Java, SQL, Bash
**Libraries:** PyTorch, DSPy, LangChain, HuggingFace, MLflow, Pandas, NumPy, SciPy, Scikit-learn, Kivy, OpenBCI
**Tools:** ROS2, MuJoCo, SLEAP, Habitat-Lab, Docker, AWS, Kubernetes, Git/GitHub, Atlassian, Arduino, PTPv2, LSL
**Domains:** RL, Multi-Agent Systems, Agentic AI, NLP, CV, Sim-to-Real, PPO/SAC, Signal Processing, Pose Estimation, Neurorobotics, Embedded Systems
