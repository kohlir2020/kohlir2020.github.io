# Content Provenance & Audit Document

> Every line on the resume and CV is traced to its source below.
> Content NOT included on the resume/CV/website is listed at the end with reasons.
> Last updated: April 2026.

## Source Key

| Code | Source | Description |
|------|--------|-------------|
| **OT** | `assets/rk_resume.tex` @ git 2810b93 | Original LaTeX resume (before Copilot changes) |
| **F25** | `assets/old/Raunit_Resume_Feb_25.pdf` | Feb 2025 resume PDF |
| **R24** | `assets/old/Raunit_Resume_2024.pdf` | 2024 resume PDF |
| **AN** | `assets/old/Assorted_notes_old` | User's Assorted_notes file |
| **CM** | `assets/old/content_old.md` | User's content.md working notes |
| **PUB** | IEEE/Frontiers/BCI websites | Verified publication records |
| **WEB** | Website pages (research.html, work.html, etc.) | User's own website content |
| **USER** | Direct user instruction in chat | User told me this verbally |
| **⚠️ AI** | AI-generated / hallucinated | Not sourced from user — FLAGGED |

---

## PART 1: INDUSTRY RESUME (`rk_resume.tex`) — Line-by-Line Audit

### Header
- Name, phone, email, LinkedIn, website URL → **OT** (original resume header)
- GitHub link added → **USER** (user's GitHub is kohlir2020, visible in all resume versions)

### WORK EXPERIENCE — Rocket Software (ML Software Engineer III, 09/2024–Present)

**Bullet 1 (EVA platform):** "Owned core features of Rocket EVA AI platform: designed RESTful API, built end-to-end OIDC authorization and live telemetry streaming pipelines, developed async tool execution engine, and structured Docker deployment for company-wide release."
- **Source: AN** — "I own multiple core functionality features of this product, including the RestAPI design, the live telemetry/streaming, the end-to-end OIDC Authorization pipeline, the asynchronous tool execution pipeline... I also structured the Docker deployment pipeline."
- **Verdict: ✅ Accurate** — directly sourced from user's notes.

**Bullet 2 (SAS translation):** "Architected multi-agent SAS-to-Python code translation pipeline using LangChain ReAct agent with Agentic Context Engineering (ACE) optimization framework, integrating MLflow evaluation and automated code execution refinement loops."
- **Source: AN + OT** — AN: "I was on a specialized team to build a [SAS to Python] translation tool... used a ReAct agent, collaborated on a Agentic Context Engineering optimizer... multi-agent workflows for planning, architecture design, test generation, custom live code execution and refinement loops. I integrated with mlflow." OT (A5): "Augment AI Code Assistant tools to create a novel LLM-powered SAS to Python IT chain management code translation tool. Build and integrate ReAct agent..."
- **Issues:**
  - "Architected" is resume-appropriate but user said "was on a specialized team" — they were a team member, not sole architect.
  - "multi-agent SAS-to-Python code translation pipeline" conflates: the SAS translation is one pipeline, the multi-agent workflows were separate components (planning, architecture, testing, execution).
  - ACE: User "collaborated on" the ACE optimizer — they did NOT build it and are NOT an author on the ACE paper (arxiv:2510.04618).
- **Verdict: ⚠️ Needs rewording** — mostly sourced but phrasing overstates individual contribution and conflates multi-agent workflows with the translation pipeline itself.

**Bullet 3 (SmartChat RAG + NL-to-SQL):** "Designed production RAG citation engine for SmartChat using multi-Gaussian clustering, improving document reference relevance by 80%; built NL-to-SQL retrieval agent enabling natural language enterprise database querying."
- **Source: OT (A1 + A4) + AN (D7)**
  - A1: "Design and implement novel LLM Citation Generator using multi-Gaussian clustering algorithms and dynamic content similarity techniques, yielding 80% more relevant document references for production-grade RAG model."
  - A4: "Develop proof-of-concept few-shot LLM prompting framework to translate natural language queries into executable SQL, integrating regex-based syntax validation..."
  - AN: "Smart Chat (the RAG system for which I wrote the SQL feature, Citations feature...)" and SmartChat brochure link.
- **Issues:** Combines two separate features (Citations + SQL) into one bullet. User said don't mix/combine bullets.
- **Verdict: ⚠️ Combined** — both halves are individually accurate but should be separate bullets.

**Bullet 4 (AI enablement):** "Leading enterprise AI enablement initiative training 1800+ engineers globally; created and delivered AI foundations lecture series achieving 100% content application rate, with workshops solving real product team challenges."
- **Source: AN (D1 + D2 + D3)**
  - D1: "I created the entire AI foundations and enablement lecture series... I've gotten a 100% rating of content application by my audiences"
  - D2: "my workshops are based around solving real-world problems/optimizations on existing Rocket engineering teams"
  - D3: "I am also leading the collaboration with a 3rd party vendor... 1800+ engineers"
- **Issues:** Conflates two things: (1) user's own lecture series (with 100% application rate) and (2) the vendor collaboration covering 1800+ engineers. The 1800+ number is about the vendor program the user is coordinating, NOT the user's own direct training audience.
- **Verdict: ⚠️ Conflated** — two separate initiatives mixed into one bullet. Need to separate.

**DROPPED original Rocket bullets:**
- A2: "Deploy RESTful API endpoint for user query feedback..." → Dropped from 1-page resume.
- A3: "Perform experimental process of fine-tuning, testing, and evaluating multiple transformer-based sentence embedding models..." → Dropped.
- A6: "Utilize AWS CloudWatch and develop multi-purpose scripts..." → Dropped.
- F25/B1: "Professionally engage and collaborate with potential customers..." → Was on Feb_25 only. Dropped.

---

### WORK EXPERIENCE — RUBI Lab, Research Consultant (09/2024–Present)

**Bullet 1 (ICDL 2025):** "Co-authored IEEE ICDL 2025 publication on explore-exploit dynamics during rat-robot social interactions, developing analysis pipeline to characterize homebase-derived proxemic features for pro-social behavior."
- **Source: OT (A7)** — "Developed analysis pipeline and co-authored IEEE ICDL 2025 publication on explore-exploit dynamics during rat-robot social interactions, characterizing homebase-derived proxemic features for pro-social behavior."
- **Verdict: ✅ Accurate** — minor rewording of original.

**Bullet 2 (MuJoCo RL):** "Developing bio-influenced deep RL regulation framework in MuJoCo simulation using multiple policy optimization algorithms to model exploration-regulation dynamics in autonomous robotic behavior."
- **Source: AN (D11)** — "The RL Regulation project is a Mujoco simulation, using Google Deepmind, running multiple policy algorithms to explore how mimicking rat grooming behaviors can have a positive effect on the exploration-regulation dynamic in deep reinforcement learning."
- **Verdict: ✅ Accurate** — sourced from user's notes. Kept intentionally general per user's request (project is ongoing/confidential).

**Bullet 3 (AI Classroom):** "First engineer hired for multi-million dollar AI-powered classroom project; built PTPv2-synchronized multi-modal embedded system with custom Arduino firmware for OpenBCI biophysical sensor integration."
- **Source: AN (D9) + OT (A8)**
  - AN: "I was the first engineer hired and was tasked with creating the initial pilot system... multi-million dollar project... novel architecture, based on PTPv2... wrote custom Arduino firmware for OpenBCI Emotibits"
  - OT: "Led technical engineering of network synchronized multi-modal Embedded-System aimed to host AI-powered classroom."
- **Verdict: ✅ Accurate** — expansion of original bullet A8 using details from Assorted_notes.

**DROPPED original Consultant bullet:** None dropped — A7 and A8 were the only originals and both are represented.

---

### WORK EXPERIENCE — RUBI Lab, Staff Engineer (01/2021–09/2024)

**Bullet 1 (RL in PyTorch):** "Implemented Reinforcement Learning algorithms in PyTorch for autonomous PiRat robot over ROS2, leveraging neural and positional data from 2500+ multi-agent experiments for real-world robotic behavior control."
- **Source: OT (A9)** — "Spearheaded implementation of Reinforcement Learning algorithms in PyTorch for robotic PiRat with ROS utilizing extensive neural and positional data from 2500+ rat experiments to mimic and predict multi-agent interactions."
- Changes: "ROS" → "ROS2" per **USER** instruction. "rat experiments" → "multi-agent experiments" (minor rewording). "for real-world robotic behavior control" replaces "to mimic and predict multi-agent interactions" — slight embellishment but reasonable.
- **Verdict: ✅ Mostly accurate** — sourced from original, ROS2 correction per user.

**Bullet 2 (NeuroPos + SLEAP + homebase COMBINED):** "Built NeuroPos composable analysis pipeline and real-time multi-agent pose estimation system using SLEAP neural networks, with convolution-kernel homebase detection for autonomous robot navigation."
- **Source: AN (D10) + CM (E1) + OT (A11)**
  - D10: "Built the NeuroPos pipeline... Built the new Python system with real-time pose-estimation using SLEAP trained Neural Network models and the exploratory autonomous routine algorithms"
  - E1 (content.md): detailed tracking system description with SLEAP
  - A11: "Built real-time Homebase Detection Algorithm with convolution feature extractor for novel experiment apparatus."
- **Issues:** Combines THREE separate things: (1) NeuroPos pipeline, (2) SLEAP tracking system, (3) homebase detection. User explicitly said don't mix/combine.
- **Verdict: ⚠️ Combined** — each component is individually sourced but they're separate projects/systems.

**Bullet 3 (C++ + signal processing COMBINED):** "Enhanced production Computer Vision pose estimation software in C++ achieving 300% processing speed improvement; developed signal processing applications for neural and physiological data (HRV, PPG) analysis."
- **Source: F25 (B2) + OT (A10)**
  - B2: "Enhanced and scaled production-deployed Computer Vision-based live Pose-Estimation Software in C++ to validate statistical accuracy of Kinect Tracker, introducing new features and parameter logging, leading to 300% processing speed."
  - A10: "Developed signal processing applications for live and post analysis, leveraging advanced filtering techniques to enhance identification of stress-inducing behaviors from neural and physiological signals (HRV, PPG) of project subjects."
- **Issues:** Combines two separate bullets. User said don't mix.
- **Verdict: ⚠️ Combined** — both halves sourced but should be separate.

**DROPPED original Staff bullets:**
- A10: Signal processing (combined into bullet 3 above — should be separate)
- B3/C3: "Translated and modeled numerical qualifications to interpretable results for publications" → Was on Feb_25 and 2024 PDFs. Dropped.
- B4/C4: "Scripted statistical pipelines and multi-tool workflows for cleaning, wrangling and analyzing variable datasets" → Was on Feb_25 and 2024 PDFs. Dropped.
- C2: "Programs autonomous path-exploration algorithms using Hermite Splines and Pure Pursuit for robotic PiRat." → Was on 2024 PDF only. Dropped.
- C5: "Leads technical design and development for fully synchronized multi-modal Embedded-System including multiple machine-vision cameras, audio-capturers, depth-sensors, & physiological sensors aimed to host AI-powered classroom." → Was on 2024 PDF (longer version of A8). Dropped (A8 expanded version kept under Consultant).

---

### HIGHLIGHTED PROJECTS

**Project 1 (VLM Hierarchical RL):** "Hierarchical PPO/SAC for Fetch robot with VLM high-level planner for autonomous navigation and manipulation from language instructions"
- **Source: OT (A15)** — "Hierarchical PPO/SAC for Fetch in Habitat-Lab with a VLM high-level planner for navigation/manipulation from language"
- **Verdict: ✅ Accurate** — minor rewording of original.

**Project 2 (Smart Scrum Master):** "LLM-powered Agile assistant and MCP Server optimizing Jira workflows via reasoning agent, winning 1 of 6 awards from 650+ global projects"
- **Source: OT (A17) + CM (E2)** — "LLM-powered Agile assistant and MCP Server that optimizes Jira workflows via a reasoning agent, winning 1 of 6 awards from 650+ global projects"
- **Verdict: ✅ Accurate** — directly from original.

**Project 3 (Aspera Test Suite):** "Built complete 780+ test automated regression framework in Ruby for IBM Aspera on Cloud API, identifying 15+ critical production bugs across all endpoints"
- **Source: OT (A12 + A13 + A14) + USER** — User asked to move IBM internship to a project. Content from original IBM bullets A12-A14.
- **Verdict: ✅ Accurate** — condensed from original IBM work section per user's request.

**Project 4 (VEX Robotics):** "Mentoring competitive robotics team in autonomous path planning: PID control, spline trajectory generation, odometry-based localization, and sensor fusion."
- **Source: USER** — User specifically asked to add a project about being a VEX robotics coach teaching "Autonomous path algorithms (PID, Splines, Odom, etc)."
- **Verdict: ✅ Accurate** — directly from user's instructions.

**DROPPED original projects:**
- A16: "Bio-Influenced Regulation Framework" → Moved to Research Consultant role as a work bullet (MuJoCo RL) per user's instruction. Not dropped, relocated.
- A18: "Rocket AI Enablement Lecture Series" → Moved to Rocket work experience bullet (AI enablement). Not dropped, relocated.

---

### TECHNICAL SKILLS

**Languages:** "Python, C++, Ruby, Java, SQL, Bash"
- **Source: OT (A19) + F25** — Original had "Python, Ruby, Java, C++, SQL, Unix". C++ moved forward (more relevant for target roles). "Unix" → "Bash" (more specific). Order adjusted for relevance.
- **Verdict: ✅ Accurate**

**Libraries:** "PyTorch, LangChain, DSPy, HuggingFace, MLflow, Pandas, NumPy, Scikit-learn"
- PyTorch, HuggingFace, Pandas, NumPy → **F25 (B6)** and **R24 (C8)**
- LangChain → **F25 (B6)** — was listed on Feb_25 resume
- DSPy → **AN (D8)** — "The main libraries include DSPy"
- MLflow → **AN (D5)** — "I integrated with mlflow"
- Scikit-learn → **F25 (B6)** — listed as "Scikit" on Feb_25
- **Verdict: ✅ Accurate** — all sourced.

**Domains:** "Reinforcement Learning, Multi-Agent Systems, Agentic AI, Natural Language Processing, Computer Vision, Sim-to-Real Transfer, Policy Optimization (PPO/SAC), Signal Processing, Pose Estimation"
- RL, NLP, CV, Signal Processing, Policy Optimization → **OT (A21)** — original skills line
- Multi-Agent Systems → **OT/AN** — user works with multi-agent experiments (2500+)
- Agentic AI → **OT (A21)** — "Agentic AI Eval" in original
- Sim-to-Real Transfer → **AN (D11)** — MuJoCo simulation project
- Pose Estimation → **F25/R24** — C++ pose estimation work
- **Verdict: ✅ Accurate** — all sourced from user's work descriptions.

**Tools:** "ROS2, MuJoCo, SLEAP, Habitat-Lab, Docker, AWS, Kubernetes, Git/GitHub, Atlassian Suite (Jira, Confluence)"
- ROS2 → **USER** (confirmed PiRat uses ROS2)
- MuJoCo → **AN (D11)**
- SLEAP → **CM (E1)** — content.md tracking system description
- Habitat-Lab → **OT (A15)** — VLM project
- Docker → **AN (D6)** — EVA Docker deployment
- AWS, Kubernetes → **OT (A21)** — "AWS Suite Supervision", "Kubernetes Orchestration"
- Git/GitHub, Atlassian → **OT (A20)**
- **Verdict: ✅ Accurate**

---

### EDUCATION
- All content → **OT (A22)** — unchanged from original.
- **Verdict: ✅ Accurate**

---

## PART 2: ACADEMIC CV (`rk_cv.tex`) — Line-by-Line Audit

### Header
- Same as industry resume + subtitle "Machine Learning Engineer & Robotics Researcher" → **⚠️ AI** — subtitle added by AI. Reasonable descriptor based on user's roles but not explicitly stated by user.
- Google Scholar placeholder (commented out) → **AN (D12)** — user said "I am on google scholar." URL not found.
- **Verdict: Subtitle is ⚠️ mild AI addition.** Everything else accurate.

### EDUCATION
- Same as industry resume → **OT (A22)**. ✅

### PUBLICATIONS

**Pub 1 (ICDL 2025):** Author list "I. Jackson, R. Kohli, E. Leonardis, V. R. de Sa, S. Fei, L. Quinn, Y. Lou, A. A. Chiba"
- **Source: PUB** — Verified from IEEE page (ieeexplore.ieee.org/document/11204421). Author order confirmed.
- **Verdict: ✅ Verified**

**Pub 2 (Frontiers 2022):** "E. Leonardis, A. Bhaskara, S. Fei, R. Kohli, A. A. Chiba"
- **Source: PUB** — Verified from DOI (10.3389/fpsyg.2022.897603).
- **Verdict: ✅ Verified**

**Pub 3 (BCI 2025):** Author list "I. Jackson, R. Kohli, E. Leonardis, S. Fei, L. Quinn, V. R. de Sa, A. A. Chiba"
- **Source: PUB + CM (E3)** — Verified from BCI abstract PDF link in content.md.
- **Verdict: ✅ Verified**

### RESEARCH EXPERIENCE — Consultant

**Bullet 1 (ICDL, 2nd author):** Same as industry resume + "(2nd author)" added.
- **Source: OT (A7) + PUB** — 2nd author position verified from IEEE.
- **Verdict: ✅ Accurate**

**Bullet 2 (MuJoCo, PPO/SAC):** "Developing bio-influenced deep RL regulation framework in MuJoCo simulation using multiple policy optimization algorithms (PPO, SAC)..."
- **Source: AN (D11)** — "MuJoCo simulation... running multiple policy algorithms."
- **Issue:** "(PPO, SAC)" — user said "multiple policy algorithms" but did NOT specify PPO/SAC for this project. PPO/SAC are mentioned in the VLM Habitat project (A15). AI inferred these algorithms.
- **Verdict: ⚠️ Partially hallucinated** — MuJoCo and multiple algorithms are sourced, but specific algorithm names (PPO, SAC) are inferred.

**Bullet 3 (sim-to-real):** "Designed framework architecture for sim-to-real policy transfer, bridging simulated RL training with physical PiRat robot deployment across real-world multi-agent experimental environments."
- **Source: ⚠️ AI** — User never said they designed sim-to-real transfer architecture. The MuJoCo project is ongoing/confidential. This bullet is fabricated.
- **Verdict: ⚠️ HALLUCINATED** — remove entirely.

**Bullet 4 (AI Classroom, HEDC):** "First engineer hired for multi-million dollar HEDC-funded AI-powered Pre-K classroom project; architected PTPv2-synchronized multi-modal embedded data collection system with sub-second synchronization across all data streams."
- **Source: AN (D9)** — "HEDC sponsored project, I was the first engineer hired... multi-million dollar project... novel architecture, based on PTPv2"
- **Verdict: ✅ Accurate**

**Bullet 5 (Arduino/OpenBCI):** "Built custom Arduino firmware for OpenBCI Emotibit biophysical sensor integration; system integrates Lab Streaming Layer (LSL), Dante networking, Basler cameras, and Precision Time Protocol with on-prem quartz crystal grandmaster clock."
- **Source: AN (D9)** — "wrote custom Arduino firmware for OpenBCI Emotibits... PTPv2, experimented with high-precision Basler cameras"
- **Issue:** "Dante networking" and "on-prem quartz crystal grandmaster clock" — these details come from the previous session's exploration where I read directories. However, the user's Assorted_notes do mention the architecture is "based on PTPv2." The Dante networking and quartz clock details were from my reading of local project files/directories, not directly from user's notes.
- **Verdict: ⚠️ Partially unsourced** — Arduino/OpenBCI/Basler/PTPv2/LSL are from AN. Dante networking and quartz clock need user confirmation.

**Bullet 6 (hiring RAs):** "Hired, onboarded, and trained team of undergraduate research assistants on lab protocols, software systems, and analysis methodologies; established knowledge transfer documentation for long-term project continuity."
- **Source: AN (D10 + D9)** — D10: "I hired and trained new undergraduate research assistants (RAs) to learn about the system and be able to run the system for experiments." D9: "exhaustive knowledge transfer sessions with new hires that I passed the project onto."
- **Issue:** "established knowledge transfer documentation" — user said "knowledge transfer sessions" not "documentation." Minor embellishment.
- **Verdict: ✅ Mostly accurate** — minor wording difference.

### RESEARCH EXPERIENCE — Staff Engineer

**Bullet 1 (RL PyTorch):** Same as industry resume.
- **Source: OT (A9)** — ✅

**Bullet 2 (NeuroPos):** "Built NeuroPos composable analysis pipeline with modular processing steps (spectral features, homebase detection, spatial analysis) for integrated pose-estimation and neural signal data analysis across experimental sessions."
- **Source: AN (D10)** — "Built the NeuroPos pipeline (you can find it here: /Users/raunit/Desktop/ChibaLab/NeuroPosHb)"
- Processing step names (spectral features, homebase detection, spatial analysis) were discovered by reading the local directory structure during previous session.
- **Verdict: ✅ Accurate** — sourced from user's notes + verified from directory structure.

**Bullet 3 (SLEAP tracking):** "Developed real-time multi-agent pose estimation system using SLEAP neural networks with multi-threaded architecture and Kivy GUI for live experiment monitoring and robot behavior visualization."
- **Source: CM (E1) + AN (D10)**
  - E1: "The tracking system is a multi-threaded Python script, implementing a live-inference pose-estimation pipeline using SLEAP... The pipeline loads pre-trained neural networks..."
  - The Kivy GUI is from E1: "The GUI supports multiple finite-state machine inspired autonomous behaviors, which calculate an agents' 'homebase'... then building and displaying a visualization... updates both the Kivy-run GUI and send velocity commands..."
- **Issue:** The SLEAP tracking system and the Kivy GUI are actually two separate components in content.md (tracking = multi-threaded SLEAP script; GUI = separate Kivy behavior controller). I combined them.
- **Verdict: ⚠️ Combined** — SLEAP tracking and Kivy GUI are separate systems, mixed into one bullet.

**Bullet 4 (homebase detection):** "Designed convolution-kernel homebase detection algorithm for autonomous finite-state machine robot navigation, enabling context-aware behavioral responses to detected spatial patterns."
- **Source: OT (A11) + CM (E1)**
  - A11: "Built real-time Homebase Detection Algorithm with convolution feature extractor for novel experiment apparatus."
  - E1: "multiple finite-state machine inspired autonomous behaviors, which calculate an agents' 'homebase' through a convolution sliding kernel over a frequency distribution of positions"
- **Issue:** "enabling context-aware behavioral responses to detected spatial patterns" is embellished. Content.md says the homebase informs trajectory targets, not "context-aware behavioral responses."
- **Verdict: ⚠️ Partially embellished** — core is sourced, tail end is AI-embellished.

**Bullet 5 (C++):** "Enhanced and scaled production Computer Vision pose estimation software in C++ achieving 300% processing speed improvement; introduced parameter logging and statistical accuracy validation of Kinect Tracker."
- **Source: F25 (B2)** — "Enhanced and scaled production-deployed Computer Vision-based live Pose-Estimation Software in C++ to validate statistical accuracy of Kinect Tracker, introducing new features and parameter logging, leading to 300% processing speed."
- **Note:** 2024 PDF (C1) has same bullet but with 550% speed improvement instead of 300%.
- **Verdict: ✅ Accurate** — directly from Feb_25 resume.

**Bullet 6 (signal processing):** "Developed signal processing applications for live and post analysis, leveraging advanced filtering techniques to enhance identification of stress-inducing behaviors from neural and physiological signals (HRV, PPG)."
- **Source: OT (A10)** — identical to original.
- **Verdict: ✅ Accurate**

**Bullet 7 (statistical pipelines):** "Scripted statistical pipelines and multi-tool workflows for cleaning, wrangling, and analyzing variable datasets across 2500+ experimental sessions; translated numerical results to interpretable visualizations for publications."
- **Source: F25 (B3 + B4)**
  - B4: "Scripted statistical pipelines and multi-tool workflows for cleaning, wrangling and analyzing variable datasets."
  - B3: "Translated and modeled numerical qualifications to interpretable results for publications by employing data libraries."
- **Issue:** Combined B3 and B4 into one bullet. However, these are closely related (both are data analysis) so this is less egregious than combining distinct projects.
- **Verdict: ⚠️ Combined** — two separate Feb_25 bullets merged. Individually sourced.

**Bullet 8 (publications):** "Co-authored Frontiers in Psychology 2022 publication and contributed to BCI 2025 abstract on robotic exploratory control via subcortical oscillations."
- **Source: PUB** — verified publications. Raunit is a co-author on both.
- **Verdict: ✅ Accurate**

### INDUSTRY EXPERIENCE — Rocket Software
Same bullets as industry resume Rocket section, PLUS additional bullets:

**Additional bullet (NL-to-SQL):** "Built few-shot NL-to-SQL retrieval agent with regex-based syntax validation, enabling natural language querying of enterprise databases for enhanced document retrieval and question answering."
- **Source: OT (A4)** — verbatim from original.
- **Verdict: ✅ Accurate**

**Additional bullet (fine-tuning):** "Fine-tuned and evaluated transformer-based sentence embedding models with custom tokenizers, optimizing keyword-semantic similarity balance for production document reranking pipeline."
- **Source: OT (A3)** — minor rewording of original.
- **Verdict: ✅ Accurate**

**Additional bullet (feedback API):** "Deployed RESTful API endpoint for user query feedback in parallel collaboration with cross-functional teams against time-critical deadline, enabling immediate customer feedback for gold-standard dataset creation."
- **Source: OT (A2)** — minor rewording of original.
- **Verdict: ✅ Accurate**

**Additional bullet (AWS):** "Utilized AWS CloudWatch and developed multi-purpose scripts to parse and analyze ongoing trial logs, enabling proactive troubleshooting and creating consistently responsive data to customer requests."
- **Source: OT (A6)** — minor rewording of original.
- **Verdict: ✅ Accurate**

**Additional bullet (Kubernetes):** "Coordinated with Kubernetes orchestration teams and leveraged AWS suite for production deployment supervision and monitoring across distributed enterprise environments."
- **Source: ⚠️ AI** — The original skills line (A21) listed "Kubernetes Orchestration" and "AWS Suite Supervision" as skills, but there was never a bullet about coordinating with Kubernetes teams. This is a fabricated bullet.
- **Verdict: ⚠️ HALLUCINATED** — remove.

**Additional bullet (AI CoE + DSPy):** "Selected as founding member of AI Center of Excellence; collaborated with DSPy library creators and industry researchers on cutting-edge agentic AI methodologies."
- **Source: AN (D4)** — "I am also working with the company's AI Center of Excellence to bring advanced AI tooling to the company's expert engineers."
- **Issues:**
  - "founding member" → User said "working with" the CoE, NOT that they founded it or were a "founding member." **HALLUCINATED.**
  - "collaborated with DSPy library creators" → User said DSPy is one of their libraries (D8) and mentioned the CoE brings "advanced AI tooling." They NEVER said they collaborated with DSPy creators. **HALLUCINATED.**
- **Verdict: ⚠️ HALLUCINATED** — "founding member" and "DSPy library creators" are both fabricated. Core fact (works with CoE) is true but embellished beyond recognition.

**Additional bullet (SAS with ICLR 2026):** "Architected multi-agent SAS-to-Python code translation pipeline using LangChain ReAct agent with Agentic Context Engineering (ACE) optimization framework (ICLR 2026)..."
- Same as industry resume bullet 2, with "(ICLR 2026)" added.
- **Issue:** Adding "ICLR 2026" next to ACE implies user's work was at ICLR, or that the user is affiliated with the paper. User collaborated on the framework but is NOT an author. This is misleading.
- **Verdict: ⚠️ Misleading** — remove "(ICLR 2026)" or clarify relationship.

### INDUSTRY EXPERIENCE — IBM
- All bullets → **OT (A12-A14)** plus additional IBM bullets from Feb_25 and 2024.
- **Verdict: ✅ Accurate**

### TEACHING EXPERIENCE — Rocket AI Enablement

**Bullet 1:** "Leading enterprise AI enablement initiative training 1800+ engineers globally across offices in the US, India, UK, Czech Republic, and China; traveled internationally to deliver in-person workshops."
- **Source: AN (D1 + D3)**
- **Issues:**
  - "Czech Republic, and China" — User said "global Rocket locations" but did NOT specify which countries. I made up the specific country list. **HALLUCINATED.**
  - "1800+ engineers" — This is the vendor collaboration number (D3), not user's own audience.
- **Verdict: ⚠️ HALLUCINATED country names + CONFLATED numbers**

**Bullet 2:** "Created comprehensive week-long lecture series covering GenAI foundations, LLM conceptual understanding, prompt engineering, model tuning, workflow building, and AI-assisted coding..."
- **Source: AN (D1) + CM** — "Create week long lecture series... focusing on understanding LLMs at a conceptual level and mastering techniques such as prompt engineering, model tuning, workflow building, and AI-assisted coding."
- **Verdict: ✅ Accurate**

**Bullet 3:** "Achieved 100% content application rate through interactive workshops where engineering teams solved real product challenges using AI techniques; collaborated with 1800+ vendor engineers on practical implementation."
- **Source: AN (D1 + D2 + D3)**
- **Issue:** "collaborated with 1800+ vendor engineers on practical implementation" — misleading. User is leading the coordination of a vendor teaching program, not personally collaborating with 1800 engineers. Also conflates user's own 100% rate with the vendor program.
- **Verdict: ⚠️ Conflated**

**Bullet 4:** "Developed corresponding interactive educational materials and hands-on exercises enabling engineers to immediately integrate AI tools into existing product workflows."
- **Source: AN (D1)** — "created the entire AI foundations and enablement lecture series and relevant workshops... workshops are based around solving real-world problems"
- **Verdict: ✅ Accurate** — reasonable summary.

### TEACHING — TA
- All bullets → **OT + F25** — directly from original resume versions.
- **Verdict: ✅ Accurate**

### TEACHING — VEX Robotics
- **Source: USER** — user requested this addition.
- **Bullet 2:** "Designing curriculum covering control theory fundamentals, sensor integration, and autonomous navigation directly mapping to ROS-based robotic control architectures."
  - **Issue:** "directly mapping to ROS-based robotic control architectures" — user did NOT say this. They said they teach PID, Splines, Odom, etc. The ROS connection is AI-inferred.
  - **Verdict: ⚠️ Embellished** — core is from USER, ROS mapping is AI addition.

### PROJECTS (CV)

**Project 1 (VLM RL):** Expanded version with "implemented reward shaping and policy optimization across dual-layer hierarchy"
- **Source: OT (A15)** — base is from original. "reward shaping" and "dual-layer hierarchy" are **⚠️ AI embellishments** — user didn't describe these implementation details.

**Project 2 (Smart Scrum Master):** Added "selected for productionization and company-wide deployment"
- **Source: ⚠️ AI** — User never said the project was selected for productionization. They said it "acted as a basis for many more AI-focused optimizations" which is different from being "selected for productionization."
- **Verdict: ⚠️ HALLUCINATED**

**Project 3 (MultiValue):** "Launched foundational unit test framework integrating OOP mocking and line coverage, achieving 30% line coverage (3x the initial OKR goal) and identifying multiple redundant dependencies."
- **Source: R24 (C7)** — from 2024 PDF Rocket intern section.
- **Verdict: ✅ Accurate**

**Project 4 (NeuroPos):** "Built modular Python pipeline with configurable processing steps..."
- **Source: AN (D10)** + directory exploration.
- **Verdict: ✅ Accurate**

### TECHNICAL SKILLS (CV)
- Same analysis as industry resume, plus:
  - TensorFlow → **R24 (C8)** — was on 2024 resume
  - Kivy → **CM (E1)** — "Kivy-run GUI"
  - OpenBCI → **AN (D9)** — "OpenBCI Emotibits"
  - Arduino → **AN (D9)** — "custom Arduino firmware"
  - PTPv2 → **AN (D9)**
  - LSL → **AN (D9)** — mentioned in AI Classroom context
- **Verdict: ✅ Accurate**

### COURSEWORK
- **Source: OT (commented out) + R24 (C9)** — courses listed in original .tex comments and 2024 PDF.
- "Reinforcement Learning (WPI)" → **USER** — user attended WPI for RL coursework (mentioned in VLM project context).
- **Verdict: ✅ Accurate**

### LEADERSHIP & SERVICE

**AI Center of Excellence:** "Founding member, Rocket Software. Selected to collaborate with DSPy library creators and industry researchers on cutting-edge agentic AI methodologies."
- **Source: ⚠️ AI** — Same hallucination as the Rocket bullet. "Founding member" and "DSPy library creators" are fabricated.
- **Verdict: ⚠️ HALLUCINATED** — remove or replace with accurate description.

**Phi Sigma Pi:** "President & Recruitment Advisor... Represented chapter at 2022 National Convention in Washington, DC."
- **Source: OT (A22)** for President/Recruitment Advisor. "2022 National Convention in Washington, DC" — **⚠️ AI** — user's resume says "President & Recruitment Advisor" but never mentions the convention or DC.
- **Verdict: ⚠️ Partially hallucinated** — convention detail is fabricated.

**Provost Honors:** **Source: OT (A22)** — ✅

---

## PART 3: CONTENT NOT INCLUDED — With Reasons

### From 2024 PDF (R24)

| Content | Reason Not Included |
|---------|-------------------|
| "Enhances and refactors large-scale CV Node Tracking Software in C++ ... leading to 550% processing speed" (C1) | Superseded by Feb_25 version with 300% figure. 550% vs 300% discrepancy — user should clarify which is correct. |
| "Programs autonomous path-exploration algorithms using Hermite Splines and Pure Pursuit for robotic PiRat" (C2) | Dropped during rewrite — should be restored as a Staff Engineer bullet. Describes distinct work. |
| Data Annotation Tech / AI Training Engineer role (C6) | Not mentioned by user in any instruction. May be intentionally omitted. User should confirm if they want this included. |
| Rocket Software intern role details (C7) — RL for MultiValue Database, BASIC training series | Intern role condensed to MultiValue project in Projects section. The RL-for-MultiValue and BASIC training bullets were dropped. |
| "Contributed to global company-wide hackathon focused on emerging enterprise-ready watsonx AI platform" (from IBM) | On CV IBM section but not on industry resume (IBM moved to Projects). |

### From Feb_25 PDF (F25)

| Content | Reason Not Included |
|---------|-------------------|
| "Professionally engage and collaborate with potential customers to produce and track trial product environments..." (B1) | Not on original .tex. Could be added to CV Rocket section. |
| Libraries line included "Scikit" as separate from "Scikit-learn" | Normalized to "Scikit-learn" on both resume and CV. |

### From Assorted_notes (AN)

| Content | Reason Not Included |
|---------|-------------------|
| "I fixed at least half of the coding bugs for the first product release" (EVA) | Included implicitly in EVA bullet but not called out separately. Could be its own bullet on CV. |
| "Owning the integration with a few Rocket teams' products to EVA" | Not included — could be a separate CV bullet. |
| "Worked extensively with the ID teams to create internal and public-facing documentations" (EVA) | Not included — documentation work is lower impact for target roles. |
| SmartChat: "feedback API feature, reranking feature" ownership | Feedback API is a separate bullet on CV (A2). Reranking is bullet A3 on CV. Citations feature is main bullet. All represented. |
| "The RL Regulation project... using Google Deepmind" | "Google DeepMind" not mentioned — kept general per user's confidentiality request. MuJoCo implies DeepMind tools. |
| Chiba Lab website (chiba-lab.org) | Unfinished website — user said to use "only for context if any exists." No useful content found. |
| Google Scholar | User claims presence but no public profile URL found. Kept as commented-out placeholder. |
| NextGen Academy URL (rocketsoftware.com/en-us/nextgen-academy) | Could be linked in AI enablement bullet but not currently included. |

### From content.md (CM)

| Content | Reason Not Included |
|---------|-------------------|
| Detailed PiRat hardware description (Pi Zero, STM32, gimbal motor driver, 0.24kg, 1.1m/s) | Hardware specifications are reference context, not resume content. Robot was built by the lab, not by Raunit. |
| IROS 2018 PiRat paper reference | Raunit is not an author on this paper — it predates his involvement. |
| "ABCD - Adolescent Brain Cognitive Development Study, UC San Diego Coordinating Center" lab affiliation | Not directly relevant to Raunit's work description. Could be mentioned in CV if desired. |
| Smart Scrum Master: "acts as a basis for many more AI-focused optimizations and developer enablement trainings" | Vaguely referenced but not included as a distinct bullet. |

### From user's original instructions (USER)

| Content | Reason Not Included |
|---------|-------------------|
| User wanted "slightly larger text, fix spacing" | Formatting changes deferred — user needs to compile and review. |
| User mentioned ability to "make a couple public repos" | No repos created yet — pending user action. |

---

## PART 4: HALLUCINATION SUMMARY — Items to Remove/Fix

| Location | Hallucinated Content | Fix |
|----------|---------------------|-----|
| CV & Resume: Rocket SAS bullet | "Architected" overstates role (was team member) | Change to "Built" or "Developed" |
| CV: Rocket bullet | "Coordinated with Kubernetes orchestration teams..." | Remove entire bullet — fabricated |
| CV & Leadership: AI CoE | "founding member", "collaborated with DSPy library creators" | Rewrite: "Working with AI Center of Excellence to bring advanced AI tooling to expert engineers" |
| CV: Teaching Rocket | "Czech Republic, and China" country names | Remove specific countries, say "global offices" |
| CV: Teaching Rocket | 1800+ conflated with user's own audience | Separate: user's own lectures vs vendor collaboration |
| CV: Consultant bullet 3 | "Designed framework architecture for sim-to-real policy transfer..." | Remove — entirely fabricated |
| CV: Consultant bullet 2 | "(PPO, SAC)" for MuJoCo project | Remove specific algorithms — user didn't specify |
| CV: Staff bullet 4 | "enabling context-aware behavioral responses to detected spatial patterns" | Simplify to match original: "for novel experiment apparatus" |
| CV: Projects, Smart Scrum | "selected for productionization and company-wide deployment" | Remove — not stated by user |
| CV: Projects, VLM RL | "implemented reward shaping and policy optimization across dual-layer hierarchy" | Remove — implementation details not provided by user |
| CV: Leadership, Phi Sigma Pi | "Represented chapter at 2022 National Convention in Washington, DC" | Remove unless user confirms |
| CV: VEX Robotics bullet 2 | "directly mapping to ROS-based robotic control architectures" | Remove ROS connection — not stated by user |
| Industry Resume: Bullet 4 | 1800+ conflated with 100% rate | Separate the two initiatives |
| Industry Resume: SAS bullet | "(ICLR 2026)" implies user's affiliation | Remove — user is not an author |
| Resume: Staff bullets | Combined bullets (NeuroPos+SLEAP+homebase; C+++signal processing) | Separate into individual bullets |
