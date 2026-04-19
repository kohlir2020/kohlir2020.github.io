Work:
- RAG Citation Generator
    - Design and implement novel Large Language Model Citation Generator using multi-Gaussian clustering algorithms and dynamic content similarity techniques, yielding 80% more relevant document references for production-grade RAG model.
- SQL Retrieval Agent
    - Develop proof-of-concept few-shot LLM prompting framework to translate natural language queries into executable SQL, integrating regex-based syntax validation, enhancing table-based document retrieval and question answering.
- SAS Code Translation Agent
    - Augment state-of-the-art AI Code Assistant tools to create a novel LLM-powered SAS to python IT chain management code translation tool. Build and integrate Retrieval and Action (ReAct) agent for SAS code analysis and equivalent python architecture generation to guide agentic translation pipeline.
- Upskilling the Workplace with AI Skills
    - Create week long lecture series and corresponding interactive educational material for both company internship program and company-wide audience aimed at providing general overview of GenAI and focusing on how to use AI to optimize one's workday. Collaborates with educational team and delivers lecture series, focusing on understanding LLMs at a conceptual level and mastering techniques such as prompt engineering, model tuning, workflow building, and AI-assisted coding. 
- Smart Scrum Master - 2025 Rocket.Build Hackathon Finalist
    - Create an LLM-powered application that interfaces with daily Atlassian developer tools to optimize agile scrum rituals aimed to organize, augment, and track team workload, progress, and velocity.
- Aspera API Test Integration
    - Scripted in Ruby to automate API endpoint testing for entire IBM Aspera on Cloud Workflows App designed to automate workflows of global content transfer and exchange across on-premises and multi-cloud environments.
    - Developed and documented comprehensive automated regression framework with 780+ API tests covering all endpoints.
    - Identified 15+ critical issues and bugs on live production server, communicated with developers to determine ideal expected behavior, and raised issues in project management tools to expertly report relevant failure details.
    - Executed full development cycle to outline and implement API Endpoint Test Controller for collaborative QA repository.
- MultiValue Experience Unit Test Coverage

Research:

- publication: https://openlib.tugraz.at/download.php?id=686289f5ddb80&location=browse

- Pirat Homebase
    - Robotics Using Bayesian Inference Lab 
    - Chiba Lab
- Pirat RL Regulation Optimization
    - Robotics Using Bayesian Inference Lab 
    - Chiba Lab
- AI Classroom
    - Center for Human Development
    - Cognitive Science Department
    - ABCD - Adolescent Brain Cognitive Development Study, UC San Diego Coordinating Center


Pirat Research Tech Stack:
This study tests whether interaction with a mobile robot “PiRat” alters homebase dynamics compared with solo exploration and conspecific dyads exploration of rats. The experiment utilizes a custom-built software and mechanical stack consisting of a novel rat-sized robot, an in-house built production-scale live multi-agent pose estimation pipeline, and a lab-built ROS-powered autonomous robotic behavior controller software. The CS-related experimental question revolves around optimizing the tech stack and debugging the entire autonomous robotic behavior and data collection process during trials. 
PiRat electronics consist of three circuit boards stacked one on top of the other having an identical footprint to that of a Raspberry Pi Zero (Pi Zero), The top board in the stack is the Pi Zero (running Raspbian), allowing PiRat to connect to Wi-Fi networks through its inbuilt wireless card. The Pi Zero is connected to the distribution board through a novel USB connector that slots in at a right-angle to the other two boards. The second board (the distribution board) contains an STM32 F042 microcontroller that handles the USB connection to the Pi Zero, PWM connections to magnetic wheel encoders and a USART connection to the third circuit board. The third circuit board (the driver board) is a custom-made two gimbal motor driver based on Martinez Gimbal board that generates the control signals for PiRat’s gimbal motors. Software on PiRat is minimal. The Pi Zero uses Robot Operating System (ROS) to communicate with a tracking system and behaviour manager. Translational and angular velocities are forwarded from the Pi Zero to the gimbal motors. PiRat weighs 0.24kg, has a top speed of 1.1m/s and a top angular velocity of 4.7m/s [Robotics lab; Rat lab. PiRat: An autonomous framework for studying social behaviour in rats and robots. Rep U S. 2018 Oct;2018:7601-7608. doi: 10.1109/iros.2018.8594060. Epub 2019 Jan 7. PMID: 34621592; PMCID: PMC8492938.]. 
PiRat is controlled by an external GUI software, built entirely in Python, which captures live global top-down positions of all agents in the circular arena and calculates a target linear and angular velocity based on PiRat's position and orientation relative to a pre-assigned target. The GUI supports multiple finite-state machine inspired autonomous behaviors, which calculate an agents' "homebase" through a convolution sliding kernel over a frequency distribution of positions, then defines an immediate target position as the immediate next pose on a trajectory that either intersects or circumvents the homebase. Behaviors then update both the Kivy-run GUI and send velocity commands to the PiRat via ROS. 
The tracking system is a multi-threaded Python script, implementing a live-inference pose-estimation pipeline using SLEAP (Social LEAP Estimates Animal Poses). The pipeline loads pre-trained neural networks, then enters a trial-length loop of capturing RGB frames from the main arena camera, feeding them into an inference calculation using the loaded models, pushing the estimated agent poses into a dynamic memory array, then building and displaying a visualization of the pose estimates over the captured frames. Poses are streamed to the behavior-controlling GUI software in real-time. 

Rocket Build Project:
My team and I were finalists for the 2025 gloabl Rocket.Build hackathon. We won the Most Innovative Project award at Rocket.Build, one of 6 winning projects out of over 650 projects worldwide. The project was called Smart Scrum Master. Our project is a brand new Agile assistant tool which optimized Jira workflows by securely updating/creating/searching/summarizing Jira tickets based on user queries or content from a Teams meeting. It uses a reasoning Agent to intelligently organize a team's Jira board, find relevant information, and update tasks, saving teams many hours throughout the week. It also exposed itself as an MCP Server and can be hosted by other chatbots and IDEs to allow Jira and Teams meeting content to directly show up in a developer's coding environment and act as essential context. The project acted as a basis for many more AI-focused optimizations and developer enablement trainings that I implemeted throughout the next six months. [clean this up]