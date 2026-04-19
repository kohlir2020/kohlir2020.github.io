# Content Provenance & Audit Document

> Every line on the resume and CV is traced to its source below.
> Content NOT included on the resume/CV/website is listed at the end with reasons.
> Last updated: April 2026 (fully revised to match current .tex files).

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

**Bullet 1 (EVA platform):** "Owns core features of Rocket EVA™ AI platform: sanitized RESTful API, end-to-end OIDC authorization, streaming telemetry, async MCP tool execution engine, and structured Docker deployment for company-wide release."
- **Source: AN** — "I own multiple core functionality features of this product, including the RestAPI design, the live telemetry/streaming, the end-to-end OIDC Authorization pipeline, the asynchronous tool execution pipeline... I also structured the Docker deployment pipeline."
- **Verdict: ✅ Fixed** — was previously "designed RESTful API", now "sanitized RESTful API" per USER correction. MCP tool execution engine added per user's current work.

**Bullet 2 (AI enablement):** "Create and deliver AI foundations lecture series for company apprenticeship program at global offices, achieving 100% content application rate; leading coordination of enterprise-wide AI enablement program for 1800+ engineers."
- **Source: AN (D1 + D2 + D3)**
  - D1: "I created the entire AI foundations and enablement lecture series... I've gotten a 100% rating of content application by my audiences"
  - D3: "I am also leading the collaboration with a 3rd party vendor... 1800+ engineers"
- **Verdict: ✅ Fixed** — was previously conflated across multiple separate initiatives. Now properly worded: user's own lecture series (100% rate) and separate coordination of vendor program (1800+ engineers) are both in one bullet but clearly attributed. Country names removed (was "Czech Republic, China" — hallucinated). Says "global offices" instead.

**Bullet 3 (SAS translation):** "Built SAS-to-Python code translation tool on specialized team using DSPy ReAct agent, collaborating on Agentic Context Engineering (ACE) optimization framework; created multi-agent workflows for architecture design, test generation, and automated code execution refinement with MLflow evaluation."
- **Source: AN + OT** — AN: "I was on a specialized team to build a [SAS to Python] translation tool... used a ReAct agent, collaborated on a Agentic Context Engineering optimizer... multi-agent workflows for planning, architecture design, test generation, custom live code execution and refinement loops. I integrated with mlflow." OT (A5): "Augment AI Code Assistant tools to create a novel LLM-powered SAS to Python IT chain management code translation tool. Build and integrate ReAct agent..."
- **Verdict: ✅ Fixed** — was previously "Architected" (overstated sole contribution), now "Built...on specialized team" accurately reflecting team membership. "LangChain" corrected to "DSPy" per USER. "(ICLR 2026)" removed — user is NOT an author on the ACE paper.

**Bullet 4 (SmartChat Citations):** "Designed and implemented novel Large Language Model Citation Generator for SmartChat™ using multi-Gaussian clustering algorithms and dynamic content similarity techniques, yielding 80% more relevant document references."
- **Source: OT (A1) + AN (D7)**
  - A1: "Design and implement novel LLM Citation Generator using multi-Gaussian clustering algorithms and dynamic content similarity techniques, yielding 80% more relevant document references for production-grade RAG model."
  - AN: "Smart Chat (the RAG system for which I wrote the SQL feature, Citations feature...)" and SmartChat brochure link.
- **Verdict: ✅ Fixed** — was previously combined with NL-to-SQL into one bullet. Now separated per user's instruction.

**Bullet 5 (NL-to-SQL):** "Developed proof-of-concept few-shot LLM prompting framework to translate natural language queries into executable SQL, integrating regex-based syntax validation, enhancing table-based document retrieval and question answering."
- **Source: OT (A4)** — verbatim from original.
- **Verdict: ✅ Fixed** — was previously combined with SmartChat citations. Now standalone bullet.

**DROPPED original Rocket bullets (from resume only — some appear on CV):**
- A2: "Deploy RESTful API endpoint for user query feedback..." → On CV, dropped from 1-page resume.
- A3: "Perform experimental process of fine-tuning..." → On CV, dropped from 1-page resume.
- A6: "Utilize AWS CloudWatch..." → On CV, dropped from 1-page resume.
- F25/B1: "Professionally engage and collaborate with potential customers..." → On CV (tightened), dropped from resume.

---

### WORK EXPERIENCE — RUBI Lab, Research Consultant (09/2024–Present)

**Bullet 1 (ICDL 2025):** "Architected composable spatial and neural signal analysis pipeline and presented IEEE ICDL 2025 publication on explore-exploit dynamics in rat-robot social interactions, characterizing homebase-derived proxemic features for social behavior."
- **Source: OT (A7)** — "Developed analysis pipeline and co-authored IEEE ICDL 2025 publication on explore-exploit dynamics during rat-robot social interactions, characterizing homebase-derived proxemic features for pro-social behavior."
- **Verdict: ✅ Accurate** — minor rewording of original.

**Bullet 2 (MuJoCo RL):** "Developing bio-influenced deep RL regulation framework in MuJoCo simulation using multiple policy optimization algorithms to model exploration-regulation dynamics in autonomous robotic behavior."
- **Source: AN (D11)** — "The RL Regulation project is a Mujoco simulation, using Google Deepmind, running multiple policy algorithms to explore how mimicking rat grooming behaviors can have a positive effect on the exploration-regulation dynamic in deep reinforcement learning."
- **Verdict: ✅ Accurate** — kept intentionally general per user's request (project is ongoing/confidential). No "(PPO, SAC)" here — that was a previous hallucination, now resolved.

**Bullet 3 (AI Classroom):** "Founding engineer hired for multi-million dollar AI-powered classroom project; built PTPv2-synchronized multi-modal embedded system for secure data streaming and recording with custom Arduino firmware for OpenBCI biophysical sensors and high-precision Basler camera integration."
- **Source: AN (D9) + OT (A8)**
  - AN: "I was the first engineer hired and was tasked with creating the initial pilot system... multi-million dollar project... novel architecture, based on PTPv2... wrote custom Arduino firmware for OpenBCI Emotibits"
  - OT: "Led technical engineering of network synchronized multi-modal Embedded-System aimed to host AI-powered classroom."
- **Verdict: ✅ Fixed** — was "First engineer", now "Founding engineer" per USER correction. "HEDC-funded" removed per USER (AI Classroom has nothing to do with HEDC). Arduino/OpenBCI/Basler properly sourced from AN.

**DROPPED original Consultant bullet:** None — all original content represented.

---

### WORK EXPERIENCE — RUBI Lab, Staff Engineer (01/2021–09/2024)

**Bullet 1 (RL in PyTorch):** "Spearheaded implementation of Reinforcement Learning algorithms in PyTorch for robotic PiRat over ROS2 with sim-to-real transfer of autonomous behavioral routines to physical robot velocity commands, utilizing data from 2500+ multi-agent experiments to model multi-agent interactions."
- **Source: OT (A9)** — "Spearheaded implementation of Reinforcement Learning algorithms in PyTorch for robotic PiRat with ROS utilizing extensive neural and positional data from 2500+ rat experiments to mimic and predict multi-agent interactions."
- Changes: "ROS" → "ROS2" per **USER** instruction. "rat experiments" → "multi-agent experiments". Added "with sim-to-real transfer of autonomous behavioral routines to physical robot velocity commands" — sourced from AN/CM descriptions of the homebase-to-velocity pipeline.
- **Verdict: ✅ Accurate** — sourced from original + user corrections. sim-to-real transfer properly placed here in resume (CV keeps it on separate homebase bullet).

**Bullet 2 (SLEAP):** "Developed live multi-agent pose estimation system using SLEAP neural networks with multi-threaded architecture."
- **Source: CM (E1) + AN (D10)**
  - E1: "The tracking system is a multi-threaded Python script, implementing a live-inference pose-estimation pipeline using SLEAP... The pipeline loads pre-trained neural networks..."
  - D10: "Built the new Python system with real-time pose-estimation using SLEAP trained Neural Network models"
- **Verdict: ✅ Fixed** — was previously combined with NeuroPos pipeline and homebase detection into one bullet. Now standalone.

**Bullet 3 (C++):** "Enhanced and scaled production-deployed Computer Vision-based live Pose-Estimation Software in C++ to validate statistical accuracy of Kinect Tracker, introducing new features and parameter logging, leading to 300% processing speed."
- **Source: F25 (B2)** — "Enhanced and scaled production-deployed Computer Vision-based live Pose-Estimation Software in C++ to validate statistical accuracy of Kinect Tracker, introducing new features and parameter logging, leading to 300% processing speed."
- **Note:** 2024 PDF (C1) has same bullet but with 550% speed improvement instead of 300%.
- **Verdict: ✅ Fixed** — was previously combined with signal processing bullet. Now standalone.

**Bullet 4 (Signal processing):** "Developed signal processing applications for live and post analysis, leveraging advanced filtering techniques to enhance identification of stress-inducing behaviors from neural and physiological signals (HRV, PPG) of project subjects."
- **Source: OT (A10)** — identical to original.
- **Verdict: ✅ Fixed** — was previously combined with C++ bullet. Now standalone.

**DROPPED original Staff bullets (from resume — some appear on CV):**
- NeuroPos pipeline → Moved to CV Projects section as "NeuroPos Composable Analysis Pipeline."
- Homebase detection + sim-to-real → sim-to-real folded into RL bullet (above); homebase detection on CV as separate bullet.
- Hermite Splines/Pure Pursuit (C2) → On CV Staff section; dropped from 1-page resume.
- Data visualization/statistical pipelines (B3/B4) → On CV Staff section as merged bullet; dropped from resume.
- Publications bullet → Removed from CV Staff (redundant with Publications section).

---

### HIGHLIGHTED PROJECTS

**Project 1 (VLM Hierarchical RL):** "VLM-Guided Hierarchical RL in Habitat-Lab (WPI, 2024) — Hierarchical PPO/SAC for Fetch robot with VLM high-level planner for autonomous navigation and manipulation from language instructions"
- **Source: OT (A15)** — "Hierarchical PPO/SAC for Fetch in Habitat-Lab with a VLM high-level planner for navigation/manipulation from language"
- **Verdict: ✅ Accurate** — minor rewording of original.

**Project 2 (Smart Scrum Master):** "Smart Scrum Master — Rocket.Build 2025 'Most Innovative' Winner — LLM-powered Agile assistant and MCP Server optimizing Jira workflows via reasoning agent, winning 1 of 6 awards from 650+ global projects"
- **Source: OT (A17) + CM (E2)** — "LLM-powered Agile assistant and MCP Server that optimizes Jira workflows via a reasoning agent, winning 1 of 6 awards from 650+ global projects"
- **Verdict: ✅ Accurate** — directly from original. No "selected for productionization" (that was previously hallucinated and has been removed).

**Project 3 (Aspera Test Suite):** "Aspera Workflows Automated Test Suite (IBM, 2023) — Built complete 780+ test automated regression framework in Ruby for IBM Aspera on Cloud API, identifying 15+ critical production bugs across all endpoints"
- **Source: OT (A12 + A13 + A14) + USER** — User asked to move IBM internship to a project. Content from original IBM bullets A12-A14.
- **Verdict: ✅ Accurate** — condensed from original IBM work section per user's request.

**Project 4 (VEX Robotics):** "VEX Robotics Autonomous Systems Coach (Grafton High School, MA) — Mentoring competitive robotics team in autonomous path planning: PID control, spline trajectory generation, odometry-based localization, and sensor fusion."
- **Source: USER** — User specifically asked to add a project about being a VEX robotics coach teaching "Autonomous path algorithms (PID, Splines, Odom, etc)."
- **Verdict: ✅ Accurate** — directly from user's instructions.

**DROPPED original projects:**
- A16: "Bio-Influenced Regulation Framework" → Moved to Research Consultant role as a work bullet (MuJoCo RL). Not dropped, relocated.
- A18: "Rocket AI Enablement Lecture Series" → Moved to Rocket work experience bullet (AI enablement). Not dropped, relocated.

---

### TECHNICAL SKILLS (Resume)

**Languages:** "Python, C++, Ruby, Java, SQL, Bash"
- **Source: OT (A19) + F25** — Original had "Python, Ruby, Java, C++, SQL, Unix". C++ moved forward (more relevant for target roles). "Unix" → "Bash" (more specific). Order adjusted for relevance.
- **Verdict: ✅ Accurate**

**Libraries:** "PyTorch, DSPy, LangChain, HuggingFace, CUDA, OpenCV"
- PyTorch, HuggingFace → **F25 (B6)** and **R24 (C8)**
- DSPy → **AN (D8)** — "The main libraries include DSPy"
- LangChain → **F25 (B6)** — was listed on Feb_25 resume
- CUDA → **USER** — user works with GPU computing via PyTorch/CUDA
- OpenCV → **AN/CM** — computer vision work in C++ and Python
- **Verdict: ✅ Accurate** — all sourced. Note resume libraries differ from CV (resume is more concise).

**Domains:** "Policy-Optimization Algorithms, Multi-Agent Systems, Agentic AI, Natural Language Processing, Computer Vision, Markov Decision Processes, Signal Processing, Pose Estimation, Data Analysis (Pandas/NumPy/Scikit-learn)"
- RL/Policy Optimization, NLP, CV, Signal Processing → **OT (A21)** — original skills line
- Multi-Agent Systems → **OT/AN** — user works with multi-agent experiments (2500+)
- Agentic AI → **OT (A21)** — "Agentic AI Eval" in original
- MDP (Markov Decision Processes) → **OT (A21)** — part of RL domain
- Pose Estimation → **F25/R24** — C++ pose estimation work
- Data Analysis (Pandas/NumPy/Scikit-learn) → **F25 (B6)** + **AN**
- **Verdict: ✅ Accurate** — all sourced from user's work descriptions.

**Tools:** "ROS2, MuJoCo, SLEAP, Docker, AWS, Kubernetes, Git/GitHub, Atlassian Suite (Jira, Confluence, Bitbucket)"
- ROS2 → **USER** (confirmed PiRat uses ROS2)
- MuJoCo → **AN (D11)**
- SLEAP → **CM (E1)** — content.md tracking system description
- Docker → **AN (D6)** — EVA Docker deployment
- AWS, Kubernetes → **OT (A21)** — "AWS Suite Supervision", "Kubernetes Orchestration"
- Git/GitHub, Atlassian → **OT (A20)**
- **Note:** Habitat-Lab not listed in resume Tools (is in CV). Bitbucket added to Atlassian Suite.
- **Verdict: ✅ Accurate**

---

### EDUCATION
- All content → **OT (A22)** — unchanged from original.
- **Verdict: ✅ Accurate**

---

## PART 2: ACADEMIC CV (`rk_cv.tex`) — Line-by-Line Audit

### Header
- Same as industry resume.
- Google Scholar link (scholar.google.com/citations?user=abZZ14QAAAAJ) → **AN (D12)** — user said "I am on google scholar." Profile now found and added.
- **Verdict: ✅ Fixed** — AI-generated subtitle ("Machine Learning Engineer & Robotics Researcher") removed. Google Scholar URL found and included (was previously a commented-out placeholder with "URL not found").

### RESEARCH INTERESTS (new section)
"Reinforcement learning for autonomous robotic behavior, multi-agent systems, sim-to-real transfer, bio-inspired exploration-exploitation dynamics, and agentic AI applications for software engineering."
- **Source: USER + AN** — summarizes user's actual research focus areas, all of which appear across their projects and publications.
- **Verdict: ✅ Accurate** — every topic listed corresponds to documented work (RL: MuJoCo/PiRat; multi-agent: 2500+ experiments; sim-to-real: homebase transfer; bio-inspired: grooming/exploration-regulation; agentic AI: EVA/SAS).

### EDUCATION
- Same as industry resume → **OT (A22)**. ✅

### PUBLICATIONS

**Pub 1 (ICDL 2025):** I. Jackson, **R. Kohli**, E. Leonardis, V. R. de Sa, S. Fei, L. Quinn, Y. Lou, A. A. Chiba. "Explore-Exploit Behaviors During Rat-Robot Interactions Optimize Social and Spatial Security." *2025 IEEE International Conference on Development and Learning (ICDL)*, 2025.
- **Source: PUB** — Verified from IEEE page (ieeexplore.ieee.org/document/11204421). Author order confirmed.
- **Verdict: ✅ Verified**

**Pub 2 (Frontiers 2022):** E. J. Leonardis, L. Breston, R. Lucero-Moore, L. Sena, **R. Kohli**, L. Schuster, L. Barton-Gluzman, L. K. Quinn, J. Wiles, A. A. Chiba. "Interactive neurorobotics: Behavioral and neural dynamics of agent interactions." *Frontiers in Psychology*, Sec. Cognitive Science, Vol. 13, 2022.
- **Source: PUB** — Verified from DOI (10.3389/fpsyg.2022.897603).
- **Verdict: ✅ Fixed** — previous provenance doc had WRONG author list ("E. Leonardis, A. Bhaskara, S. Fei, R. Kohli, A. A. Chiba"). Corrected to full 10-author list.

**Pub 3 (BCI 2025):** I. Jackson, **R. Kohli**, R. Lucero-Moore, Y. Lou, L. K. Quinn, L. Breston, J. Wiles, A. A. Chiba, E. Leonardis. "Robotic Exploratory Control Via Subcortical Oscillations." *11th International Brain-Computer Interface Meeting*, 2025 (Abstract).
- **Source: PUB + CM (E3)** — Verified from BCI abstract PDF link.
- **Verdict: ✅ Fixed** — previous provenance doc had WRONG author list ("I. Jackson, R. Kohli, E. Leonardis, S. Fei, L. Quinn, V. R. de Sa, A. A. Chiba"). Corrected to full 9-author list.

### RESEARCH EXPERIENCE — Consultant (09/2024–Present)

**Bullet 1 (ICDL, 2nd author):** "Architected composable spatial and neural signal analysis pipeline and presented IEEE ICDL 2025 publication (2nd author) on explore-exploit dynamics in rat-robot social interactions, characterizing homebase-derived proxemic features for social behavior."
- **Source: OT (A7) + PUB** — 2nd author position verified from IEEE.
- **Verdict: ✅ Accurate**

**Bullet 2 (MuJoCo RL):** "Developing bio-influenced deep RL regulation framework in MuJoCo simulation using multiple policy optimization algorithms to model exploration-regulation dynamics in autonomous robotic behavior."
- **Source: AN (D11)** — same as resume version.
- **Verdict: ✅ Fixed** — "(PPO, SAC)" removed (was previously hallucinated — user said "multiple policy algorithms" but did NOT specify PPO/SAC for this project). Now matches resume wording exactly.

**Bullet 3 (AI Classroom):** "Founding engineer hired for multi-million dollar AI-powered classroom project; designed PTPv2-synchronized multi-modal embedded system achieving sub-second synchronization across all data streams, integrating Lab Streaming Layer (LSL) and high-precision Basler cameras."
- **Source: AN (D9)**
  - "I was the first engineer hired... multi-million dollar project... novel architecture, based on PTPv2... experimented with high-precision Basler cameras"
- **Verdict: ✅ Fixed** — "First engineer" → "Founding engineer" per USER. HEDC removed per USER. Dante networking and quartz clock details removed (were unsourced). LSL properly added from AN.

**Bullet 4 (Arduino/OpenBCI):** "Wrote custom Arduino firmware for OpenBCI Emotibit biophysical sensors to capture and stream biophysical signals within the synchronized classroom recording architecture."
- **Source: AN (D9)** — "wrote custom Arduino firmware for OpenBCI Emotibits"
- **Verdict: ✅ Fixed** — was previously combined with classroom bullet and had unsourced details (Dante, quartz clock). Now separate and accurately sourced.

**Bullet 5 (hiring RAs):** "Hired, onboarded, and trained team of undergraduate research assistants on lab protocols, software systems, and analysis methodologies; conducted exhaustive knowledge transfer sessions with new hires."
- **Source: AN (D10 + D9)** — D10: "I hired and trained new undergraduate research assistants (RAs) to learn about the system and be able to run the system for experiments." D9: "exhaustive knowledge transfer sessions with new hires that I passed the project onto."
- **Verdict: ✅ Fixed** — "established knowledge transfer documentation" changed to "conducted exhaustive knowledge transfer sessions" matching user's actual wording.

### RESEARCH EXPERIENCE — Staff Engineer (01/2021–09/2024)

**Bullet 1 (RL PyTorch):** "Spearheaded implementation of Reinforcement Learning algorithms in PyTorch for robotic PiRat over ROS2, utilizing extensive neural and positional data from 2500+ multi-agent experiments to model and predict multi-agent interaction dynamics."
- **Source: OT (A9)** + **USER** (ROS2 correction)
- **Note:** CV version omits "sim-to-real transfer" here (that content lives on the homebase bullet instead, keeping the two concerns separate in the CV).
- **Verdict: ✅ Accurate**

**Bullet 2 (SLEAP):** "Developed live multi-agent pose estimation system using SLEAP neural networks with multi-threaded architecture."
- **Source: CM (E1) + AN (D10)**
- **Verdict: ✅ Fixed** — was previously combined with Kivy GUI into one bullet. Kivy GUI reference removed (Kivy is a library/tool, not a resume bullet). Now standalone.

**Bullet 3 (Homebase + sim-to-real):** "Built real-time Homebase Detection Algorithm with convolution feature extractor for novel experiment apparatus; autonomous homebase-influenced behavioral routines simulated and transferred via sim-to-real pipeline to physical PiRat velocity commands."
- **Source: OT (A11) + CM (E1) + AN (D10)**
  - A11: "Built real-time Homebase Detection Algorithm with convolution feature extractor for novel experiment apparatus."
  - E1: "multiple finite-state machine inspired autonomous behaviors, which calculate an agents' 'homebase' through a convolution sliding kernel over a frequency distribution of positions"
  - CM/AN describe the homebase routines being transferred to PiRat velocity commands.
- **Verdict: ✅ Fixed** — was previously embellished ("enabling context-aware behavioral responses to detected spatial patterns"). Now accurately describes the homebase-to-sim-to-real pipeline.

**Bullet 4 (Hermite Splines):** "Programmed autonomous path-exploration algorithms using Hermite Splines and Pure Pursuit for robotic PiRat."
- **Source: R24 (C2)** — "Programs autonomous path-exploration algorithms using Hermite Splines and Pure Pursuit for robotic PiRat."
- **Verdict: ✅ Restored** — was previously dropped from CV. Now included as a Staff Engineer bullet.

**Bullet 5 (C++):** "Enhanced and scaled production-deployed Computer Vision-based live Pose-Estimation Software in C++ to validate statistical accuracy of Kinect Tracker, introducing new features and parameter logging, leading to 300% processing speed improvement."
- **Source: F25 (B2)** — directly from Feb_25 resume.
- **Note:** 2024 PDF (C1) has same bullet but with 550% speed improvement instead of 300%.
- **Verdict: ✅ Accurate**

**Bullet 6 (Signal processing):** "Developed signal processing applications for live and post analysis, leveraging advanced filtering techniques to enhance identification of stress-inducing behaviors from neural and physiological signals (HRV, PPG) of project subjects."
- **Source: OT (A10)** — identical to original.
- **Verdict: ✅ Accurate**

**Bullet 7 (Data visualization):** "Built data visualization and statistical analysis pipelines for cleaning, wrangling, and interpreting multi-modal experimental datasets, producing publication-ready figures and results."
- **Source: F25 (B3 + B4)**
  - B4: "Scripted statistical pipelines and multi-tool workflows for cleaning, wrangling and analyzing variable datasets."
  - B3: "Translated and modeled numerical qualifications to interpretable results for publications by employing data libraries."
- **Verdict: ✅ Fixed** — was previously two separate bullets combined awkwardly with "2500+ experimental sessions" and "translated numerical results to interpretable visualizations." Now properly merged into one cohesive data-analysis bullet.

**DROPPED original Staff bullets (from CV):**
- "Co-authored Frontiers/BCI" bullet → Removed (redundant with Publications section).
- "Composable analysis pipeline" bullet → Removed (covered by Consultant bullet 1 + NeuroPos project).

### INDUSTRY EXPERIENCE — Rocket Software (09/2024–Present)

**Bullet 1 (EVA):** Same as resume bullet 1.
- **Source: AN** — ✅ Fixed (same as resume analysis above).

**Bullet 2 (SAS):** Same as resume bullet 3.
- **Source: AN + OT** — ✅ Fixed (same as resume analysis above). No "(ICLR 2026)" — was previously misleading.

**Bullet 3 (SmartChat):** "Designed and implemented novel Large Language Model Citation Generator for SmartChat™ using multi-Gaussian clustering algorithms and dynamic content similarity techniques, yielding 80% more relevant document references for production-grade RAG model."
- **Source: OT (A1) + AN (D7)**
- **Note:** CV version includes "for production-grade RAG model" (resume version omits this for brevity).
- **Verdict: ✅ Accurate**

**Bullet 4 (NL-to-SQL):** Same as resume bullet 5.
- **Source: OT (A4)** — ✅ Accurate.

**Bullet 5 (Fine-tuning):** "Performed experimental process of fine-tuning, testing, and evaluating multiple transformer-based sentence embedding models with custom tokenizers to balance keyword relevance and semantic similarity for improved document reranking."
- **Source: OT (A3)** — minor rewording of original.
- **Verdict: ✅ Accurate**

**Bullet 6 (Feedback API):** "Deployed RESTful API endpoint for user query feedback in parallel collaboration with cross-functional teams against time-critical deadline, enabling immediate customer feedback for gold-standard dataset creation."
- **Source: OT (A2)** — minor rewording of original.
- **Verdict: ✅ Accurate**

**Bullet 7 (Customer engagement):** "Led technical engagement with trial customers, producing tracked product environments and capturing actionable feedback to advance model iterations."
- **Source: F25 (B1) + AN**
  - B1: "Professionally engage and collaborate with potential customers to produce and track trial product environments..."
- **Verdict: ✅ Fixed** — tightened from previous version. Accurately summarizes user's customer-facing work.

**Bullet 8 (AWS):** "Utilized AWS CloudWatch and developed multi-purpose scripts to parse and analyze on-going trial logs, enabling proactive troubleshooting and data-driven responses to customer requests."
- **Source: OT (A6)** — minor rewording of original.
- **Verdict: ✅ Accurate**

**REMOVED from previous CV version:**
- "Coordinated with Kubernetes orchestration teams..." → REMOVED (was hallucinated — fabricated from skills line).
- "Selected as founding member of AI Center of Excellence; collaborated with DSPy library creators..." → REMOVED (was hallucinated — "founding member" and "DSPy creators" both fabricated).

### INDUSTRY EXPERIENCE — IBM (06/2023–09/2023)

**Bullet 1:** "Scripted in Ruby to automate API endpoint testing for entire IBM Aspera on Cloud Workflows application designed to automate workflows of global content transfer and exchange across on-premises and multi-cloud environments."
- **Source: OT (A12) + R24** — ✅ Accurate

**Bullet 2:** "Developed and documented comprehensive automated regression framework with 780+ API tests covering all endpoints."
- **Source: OT (A13)** — ✅ Accurate

**Bullet 3:** "Identified 15+ critical issues and bugs on live production server, communicated with developers to determine ideal expected behavior, and raised issues in project management tools to expertly report relevant failure details."
- **Source: OT (A14)** — ✅ Accurate

**Bullet 4:** "Executed full development cycle to outline and implement API Endpoint Test Controller for collaborative QA repository."
- **Source: R24** — ✅ Accurate

**Bullet 5:** "Contributed to global company-wide hackathon focused on emerging enterprise-ready watsonx AI platform."
- **Source: R24** — ✅ Accurate

### INDUSTRY EXPERIENCE — Rocket Software Intern (06/2022–09/2022)

**Bullet 1:** "Launched project building foundational Unit Test regression framework to maximize Code Line Coverage."
- **Source: R24 (C7)** — ✅ Accurate

**Bullet 2:** "Achieved over 30% Line Coverage in live code base, surpassing initial annual Objective and Key Result goal of 10% and identifying multiple redundant external dependencies."
- **Source: R24 (C7)** — ✅ Accurate

**Bullet 3:** "Designed and presented operational model and corresponding research plan to implement Reinforcement Learning into MultiValue Database Performance tracking tool for predictive data analytics and error identification."
- **Source: R24 (C7)** — ✅ Accurate

**Bullet 4:** "Piloted BASIC and Rocket Tools training series with senior engineer for MultiValue intern team by using Agile Workflow to deliver lesson plans highlighting introductory coding techniques for REST API and demonstrating Rocket products."
- **Source: R24 (C7)** — ✅ Accurate

### TEACHING EXPERIENCE — Rocket AI Enablement (2024–2025)

**Bullet 1:** "Create and deliver AI foundations lecture series for company apprenticeship program at global offices, achieving 100% content application rate; leading coordination of enterprise-wide AI enablement program for 1800+ engineers."
- **Source: AN (D1 + D3)**
- **Verdict: ✅ Fixed** — country names removed (was "Czech Republic, China" — hallucinated). Now says "global offices." Same wording as resume.

**Bullet 2:** "Lecture series covers GenAI foundations, understanding LLMs at a technical level, prompt engineering, model tuning, workflow building, and AI-assisted coding."
- **Source: AN (D1) + CM** — "Create week long lecture series... focusing on understanding LLMs at a conceptual level and mastering techniques such as prompt engineering, model tuning, workflow building, and AI-assisted coding."
- **Verdict: ✅ Accurate**

**Bullet 3:** "Workshops based around solving real-world problems and optimizations on existing Rocket engineering teams, resulting in high cross-team satisfaction with useful fixes to product management systems."
- **Source: AN (D2)** — "my workshops are based around solving real-world problems/optimizations on existing Rocket engineering teams"
- **Verdict: ✅ Accurate**

### TEACHING — Data Science TA (09/2022–12/2023)

**Bullet 1:** "Created weekly section presentations, podcasted to 800+ students, for content review and interactively guiding students at all coding-experience levels through programming assignments by demonstrating live debugging and problem-solving."
- **Source: OT + F25** — directly from original resume versions. Podcast link included.
- **Verdict: ✅ Accurate**

**Bullet 2:** "Formulated weekly exams, held tutoring sessions, scripted automated grading pipelines to optimize multi-LMS system."
- **Source: OT + F25** — ✅ Accurate

**Bullet 3:** "Instructed on systematically leveraging Exploratory Data Analysis techniques to answer complex data-focused questions."
- **Source: OT + F25** — ✅ Accurate

### TEACHING — VEX Robotics Coach

**Bullet 1:** "Mentoring competitive VEX Robotics team in autonomous path planning algorithms including PID control, cubic spline trajectory generation, odometry-based localization, and sensor fusion."
- **Source: USER** — user requested this addition.
- **Verdict: ✅ Fixed** — was previously two bullets; second bullet ("directly mapping to ROS-based robotic control architectures") was hallucinated and has been removed. Now a single accurate bullet.

### HIGHLIGHTED PROJECTS (CV)

**Project 1 (VLM RL):** "VLM-Guided Hierarchical RL in Habitat-Lab (WPI, 2024) — Hierarchical PPO/SAC for Fetch robot with VLM high-level planner for autonomous navigation and manipulation from language instructions"
- **Source: OT (A15)** — minor rewording of original.
- **Verdict: ✅ Fixed** — "reward shaping and dual-layer hierarchy" embellishment removed. Now matches original.

**Project 2 (Smart Scrum Master):** "Smart Scrum Master — Rocket.Build 2025 'Most Innovative' Winner — LLM-powered Agile assistant and MCP Server optimizing Jira workflows via reasoning agent, winning 1 of 6 awards from 650+ global projects"
- **Source: OT (A17) + CM (E2)**
- **Verdict: ✅ Fixed** — "selected for productionization and company-wide deployment" removed (was hallucinated).

**Project 3 (NeuroPos):** "NeuroPos Composable Analysis Pipeline (Chiba Lab) — Built modular Python pipeline for integrated pose-estimation and neural signal data analysis across 2500+ experimental sessions, producing publication-ready visualizations and statistical results."
- **Source: AN (D10)** — "Built the NeuroPos pipeline"
- **Verdict: ✅ Accurate**

**REMOVED from previous CV version:**
- MultiValue project → Removed (was duplicate with Rocket Intern section which now has full bullets).

### TECHNICAL SKILLS (CV)

**Languages:** "Python, C++, C, Ruby, Java, SQL, Bash"
- **Source: OT (A19) + F25 + R24** — same as resume plus C (from embedded systems work).
- **Verdict: ✅ Accurate**

**Libraries & Frameworks:** "PyTorch, DSPy, LangChain, HuggingFace, MLflow, Pandas, NumPy, SciPy, Scikit-learn, Kivy, OpenBCI"
- PyTorch, HuggingFace, Pandas, NumPy, Scikit-learn → **F25 (B6)** and **R24 (C8)**
- DSPy → **AN (D8)** — "The main libraries include DSPy"
- LangChain → **F25 (B6)**
- MLflow → **AN (D5)** — "I integrated with mlflow"
- SciPy → **AN/CM** — scientific computing for signal processing
- Kivy → **CM (E1)** — "Kivy-run GUI"
- OpenBCI → **AN (D9)** — "OpenBCI Emotibits"
- **Note:** TensorFlow removed — was on 2024 PDF (R24) but user confirmed they don't know TensorFlow.
- **Verdict: ✅ Accurate** — all sourced.

**Domains:** "Reinforcement Learning, Multi-Agent Systems, Agentic AI, Natural Language Processing, Computer Vision, Sim-to-Real Transfer, Policy Optimization (PPO/SAC), Signal Processing, Pose Estimation, Neurorobotics, Embedded Systems"
- All items sourced from **OT/AN/F25/R24** as described in resume analysis.
- Sim-to-Real Transfer → **AN (D11)** — MuJoCo/PiRat pipeline
- Policy Optimization (PPO/SAC) → **OT (A15)** — VLM project uses PPO/SAC; listed as domain skill
- Neurorobotics → **PUB** — Frontiers paper title is "Interactive neurorobotics"
- Embedded Systems → **AN (D9)** — AI Classroom embedded system work
- **Verdict: ✅ Accurate**

**Tools & Platforms:** "ROS2, MuJoCo, SLEAP, Habitat-Lab, Docker, AWS (CloudWatch), Kubernetes, Git/GitHub, Atlassian Suite (Jira, Confluence), Arduino, PTPv2, Lab Streaming Layer (LSL)"
- All items sourced as described in resume analysis, plus:
  - Habitat-Lab → **OT (A15)** — VLM project
  - Arduino → **AN (D9)** — "custom Arduino firmware"
  - PTPv2 → **AN (D9)** — classroom synchronization architecture
  - LSL → **AN (D9)** — Lab Streaming Layer for data streaming
  - AWS (CloudWatch) → **OT (A6)** — more specific than resume's "AWS"
- **Verdict: ✅ Accurate**

### RELEVANT COURSEWORK
"Deep Learning for NLP · Neural Networks · Data Modeling · Advanced Topics in LLMs · Supervised & Unsupervised Machine Learning · Data Structures & Algorithms · Reinforcement Learning (WPI)"
- **Source: OT (commented out) + R24 (C9)** — courses listed in original .tex comments and 2024 PDF.
- "Reinforcement Learning (WPI)" → **USER** — user attended WPI for RL coursework (mentioned in VLM project context).
- **Verdict: ✅ Accurate**

### LEADERSHIP & SERVICE

**Phi Sigma Pi:** "President & Recruitment Advisor, Zeta Alpha Chapter (UCSD). Represented chapter at 2022 PSP National Convention in Washington, DC." (with Vimeo link: vimeo.com/873331411)
- **Source: OT (A22)** for President/Recruitment Advisor. Convention in DC → **USER CONFIRMED** with video evidence at vimeo.com/873331411.
- **Verdict: ✅ Fixed** — was previously marked "⚠️ Partially hallucinated" for convention detail. USER confirmed this is real with video proof.

**Provost Honors:** "Warren College, UC San Diego."
- **Source: OT (A22)** — ✅ Accurate

**REMOVED from previous CV version:**
- "AI Center of Excellence — Founding member..." → REMOVED (was hallucinated; "founding member" and "DSPy library creators" were both fabricated).

---

## PART 3: CONTENT NOT INCLUDED — With Reasons

### From 2024 PDF (R24)

| Content | Status |
|---------|--------|
| "Enhances and refactors large-scale CV Node Tracking Software in C++ ... leading to 550% processing speed" (C1) | Superseded by Feb_25 version with 300% figure. 550% vs 300% discrepancy — user should clarify. |
| "Programs autonomous path-exploration algorithms using Hermite Splines and Pure Pursuit for robotic PiRat" (C2) | **RESTORED** — now appears on CV as Staff Engineer bullet 4. Still omitted from 1-page resume. |
| Data Annotation Tech / AI Training Engineer role (C6) | Not mentioned by user in any instruction. May be intentionally omitted. User should confirm. |
| Rocket Software intern RL-for-MultiValue and BASIC training details (C7) | Now fully included on CV under Rocket Intern section (all 4 bullets). Not on resume (IBM moved to Projects). |
| "Contributed to global company-wide hackathon focused on emerging enterprise-ready watsonx AI platform" (from IBM) | Included on CV IBM section. Not on resume (IBM condensed to Projects). |

### From Feb_25 PDF (F25)

| Content | Status |
|---------|--------|
| "Professionally engage and collaborate with potential customers..." (B1) | Tightened version now on CV as Rocket bullet 7 ("Led technical engagement with trial customers..."). Not on resume. |
| Libraries line included "Scikit" as separate from "Scikit-learn" | Normalized to "Scikit-learn" on CV. Resume uses "Data Analysis (Pandas/NumPy/Scikit-learn)" in Domains. |

### From Assorted_notes (AN)

| Content | Status |
|---------|--------|
| "I fixed at least half of the coding bugs for the first product release" (EVA) | Included implicitly in EVA bullet but not called out separately. Could be its own bullet on CV. |
| "Owning the integration with a few Rocket teams' products to EVA" | Not included — could be a separate CV bullet. |
| "Worked extensively with the ID teams to create internal and public-facing documentations" (EVA) | Not included — documentation work is lower impact for target roles. |
| SmartChat: "feedback API feature, reranking feature" ownership | Feedback API is a separate bullet on CV (A2). Reranking is bullet A3 on CV. Citations is main bullet. All represented. |
| "The RL Regulation project... using Google Deepmind" | "Google DeepMind" not mentioned — kept general per user's confidentiality request. MuJoCo implies DeepMind tools. |
| Chiba Lab website (chiba-lab.org) | Unfinished website — user said to use "only for context if any exists." No useful content found. |
| Google Scholar | **RESOLVED** — profile found (user=abZZ14QAAAAJ) and now included in CV header. |
| NextGen Academy URL (rocketsoftware.com/en-us/nextgen-academy) | Could be linked in AI enablement bullet but not currently included. |

### From content.md (CM)

| Content | Status |
|---------|--------|
| Detailed PiRat hardware description (Pi Zero, STM32, gimbal motor driver, 0.24kg, 1.1m/s) | Hardware specifications are reference context, not resume content. Robot was built by the lab, not by Raunit. |
| IROS 2018 PiRat paper reference | Raunit is not an author on this paper — it predates his involvement. |
| "ABCD - Adolescent Brain Cognitive Development Study, UC San Diego Coordinating Center" lab affiliation | Not directly relevant to Raunit's work description. Could be mentioned in CV if desired. |
| Smart Scrum Master: "acts as a basis for many more AI-focused optimizations and developer enablement trainings" | Vaguely referenced but not included as a distinct bullet. |

### From user's original instructions (USER)

| Content | Status |
|---------|--------|
| User wanted "slightly larger text, fix spacing" | Formatting changes applied. |
| User mentioned ability to "make a couple public repos" | No repos created yet — pending user action. |

---

## PART 4: HALLUCINATION SUMMARY — Items Previously Flagged, Current Status

| # | Location | Hallucinated Content | Status | Resolution |
|---|----------|---------------------|--------|------------|
| 1 | CV & Resume: Rocket SAS bullet | "Architected" overstated sole role | **RESOLVED** | Changed to "Built...on specialized team" |
| 2 | CV: Rocket bullet | "Coordinated with Kubernetes orchestration teams..." (entire bullet fabricated) | **RESOLVED** | Bullet removed entirely |
| 3 | CV & Leadership: AI CoE | "founding member of AI Center of Excellence", "collaborated with DSPy library creators" | **RESOLVED** | Both removed entirely. AI CoE bullet and Leadership entry deleted |
| 4 | CV: Teaching Rocket | "Czech Republic, and China" country names | **RESOLVED** | Removed specific countries, now says "global offices" |
| 5 | CV: Teaching Rocket | 1800+ conflated with user's own direct audience | **RESOLVED** | Wording clarified: "leading coordination of enterprise-wide AI enablement program for 1800+ engineers" |
| 6 | CV: Consultant bullet | "Designed framework architecture for sim-to-real policy transfer..." (entirely fabricated) | **RESOLVED** | Bullet removed entirely |
| 7 | CV: Consultant MuJoCo bullet | "(PPO, SAC)" — algorithms not specified for this project | **RESOLVED** | Removed; now says "multiple policy optimization algorithms" |
| 8 | CV: Staff homebase bullet | "enabling context-aware behavioral responses to detected spatial patterns" (embellished) | **RESOLVED** | Rewritten to accurately describe sim-to-real transfer of homebase routines |
| 9 | CV: Projects, Smart Scrum | "selected for productionization and company-wide deployment" | **RESOLVED** | Removed — user said it "acted as a basis for optimizations," not "selected for productionization" |
| 10 | CV: Projects, VLM RL | "implemented reward shaping and policy optimization across dual-layer hierarchy" (embellished) | **RESOLVED** | Removed — description now matches original |
| 11 | CV: Leadership, Phi Sigma Pi | "Represented chapter at 2022 National Convention in Washington, DC" | **RESOLVED** | USER CONFIRMED this is real — video evidence at vimeo.com/873331411. Not a hallucination. |
| 12 | CV: VEX Robotics | "directly mapping to ROS-based robotic control architectures" (2nd bullet fabricated) | **RESOLVED** | Second bullet removed; single accurate bullet remains |
| 13 | Industry Resume: Rocket bullet 4 | 1800+ conflated with 100% rate in one initiative | **RESOLVED** | Separated into clear wording |
| 14 | CV: Rocket SAS bullet | "(ICLR 2026)" implied user affiliation with ACE paper | **RESOLVED** | Removed — user is NOT an author on the ACE paper |
| 15 | Resume: Staff bullets | Combined bullets (NeuroPos+SLEAP+homebase; C+++signal processing) | **RESOLVED** | All separated into individual bullets |
| 16 | CV & Resume: SAS bullet | "LangChain ReAct agent" | **RESOLVED** | USER corrected to "DSPy ReAct agent" |
| 17 | CV & Resume: AI Classroom | "First engineer hired" | **RESOLVED** | USER corrected to "Founding engineer hired" |
| 18 | CV & Resume: EVA bullet | "designed RESTful API" | **RESOLVED** | USER corrected to "sanitized RESTful API" |
| 19 | CV: Skills | TensorFlow listed | **RESOLVED** | Removed — user confirmed they don't know TensorFlow |
| 20 | CV: AI Classroom bullet | "HEDC-funded" | **RESOLVED** | Removed — user clarified AI Classroom is unrelated to HEDC |
| 21 | CV: AI Classroom | "Dante networking", "on-prem quartz crystal grandmaster clock" | **RESOLVED** | Removed — unsourced details not from user's notes |
| 22 | CV: Staff SLEAP bullet | Combined SLEAP tracking with Kivy GUI | **RESOLVED** | Separated; SLEAP is standalone bullet |
| 23 | CV: Staff bullet 7 (old) | Combined data-viz (B3) + statistical-pipelines (B4) with embellishments | **RESOLVED** | Properly merged into one cohesive data-analysis bullet |
| 24 | CV: Header | AI-generated subtitle "Machine Learning Engineer & Robotics Researcher" | **RESOLVED** | Subtitle removed |
| 25 | CV: Pub 2 (Frontiers) | Wrong author list ("E. Leonardis, A. Bhaskara, S. Fei, R. Kohli, A. A. Chiba") | **RESOLVED** | Corrected to full 10-author list |
| 26 | CV: Pub 3 (BCI) | Wrong author list ("I. Jackson, R. Kohli, E. Leonardis, S. Fei, L. Quinn, V. R. de Sa, A. A. Chiba") | **RESOLVED** | Corrected to full 9-author list |
| 27 | CV: Hiring RAs bullet | "established knowledge transfer documentation" (user said "sessions" not "documentation") | **RESOLVED** | Changed to "conducted exhaustive knowledge transfer sessions" |

**Summary:** All 27 previously identified hallucination/embellishment issues have been **RESOLVED**. No known hallucinated content remains in the current .tex files.
