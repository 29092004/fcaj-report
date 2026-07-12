---
title: "Event 2"
date: 2026-06-06
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Summary Report: "AWS Community Day - 06/06/2026"

### Event Objectives

- Provide in-depth knowledge on containerization technology (Docker), integrating Machine Learning with AWS WAF for cyber attack detection, and developing multiplayer games on cloud infrastructure.
- Introduce modern GraphRAG solutions using AWS Neptune graph database to build and store Knowledge Graphs.
- Share critical soft skills for effective teamwork and a realistic self-study roadmap to transition careers from IT Helpdesk to Senior System Administrator.

### Speakers & Topics

1. **Bao Huynh** - Topic: *Docker - A containerization technology*
2. **Le Hoang Gia Dai** - Topic: *Combining AWS WAF with Machine Learning for Cyber Attack Detection*
3. **Nguyen Quoc Bao** - Topic: *Multiplayer in the Cloud: Connecting Godot Clients with AWS*
4. **Truong Phuoc** - Topic: *How to Work in a Team Effectively*
5. **Viet Phat** - Topic: *AWS Neptune for Building a Graph Knowledge Base for GraphRAG*
6. **Vinh Tran** - Topic: *From IT Helpdesk to Senior Sysadmin: Self-Study Journey and Transition Roadmap*

---

### Key Highlights from Presentations

#### 1. Docker - A containerization technology
**Speaker:** Bao Huynh

- **Containerization vs. Virtualization Concepts:** Distinguishing traditional virtual machines (VMs) using Hypervisors from containers sharing the host OS kernel.
- **Docker Core Components:** An in-depth look at Docker Engine, Dockerfiles for environment definitions, Docker Images as blueprints, and running Docker Containers.
- **Managing Multiple Containers with Docker Compose:** How to write `docker-compose.yml` files to spin up frontend, backend, and database services simultaneously and synchronously.
- **Practical Value:** Eliminating the classic "works on my machine" problem, optimizing hardware resources, and accelerating application delivery (CI/CD).

#### 2. Combining AWS WAF with Machine Learning for Cyber Attack Detection
**Speaker:** Le Hoang Gia Dai

- **Limitations of Rule-based WAFs:** Analyzing vulnerability risks when faced with zero-day attacks or evolving cyber threat patterns.
- **Integrating Machine Learning with AWS WAF:** Anomaly detection solutions analyzing traffic in real-time using ML models.
- **Automated Protection Architecture:** Collecting logs with AWS WAF -> streaming through Amazon Kinesis Data Firehose -> storing in Amazon S3 -> invoking AWS Lambda to process logs with ML models -> automatically updating IP Set Blocklists on AWS WAF.
- **Benefits:** Proactively securing enterprise workloads against severe security threats without degrading request latency.

#### 3. Multiplayer in the Cloud: Connecting Godot Clients with AWS
**Speaker:** Nguyen Quoc Bao

- **Challenges in Multiplayer Games:** Managing latency and ensuring real-time game state synchronization between different players.
- **Connecting Godot Engine Game Clients:** Methods for using Godot to communicate with backend servers via high-performance protocols like UDP, TCP, or WebSockets.
- **Cloud Game Server Infrastructure:** Deploying Dedicated Game Servers utilizing AWS services like Amazon GameLift, Amazon ECS, or AWS App Runner.
- **Live Demo:** Visualizing characters controlled by players on the client-side, sending input signals to AWS, and synchronizing game states across other clients instantly.

#### 4. How to Work in a Team Effectively
**Speaker:** Truong Phuoc

- **Core Elements of a Successful Team:** Shared goals, open communication, mutual trust, and clear division of responsibilities.
- **Implementing Agile/Scrum Methodologies:** Formatting Daily Standups, Sprint Planning, and Retrospective sessions to maintain alignment and clear roadblocks quickly.
- **Collaboration Tools:** Leveraging Jira/Trello for task management, Slack/Discord for instant messaging, and Git/GitHub for cooperative codebase management without merge conflicts.
- **Conflict Resolution:** Treating disagreements as opportunities for growth, mastering active listening, and providing constructive feedback.

#### 5. AWS Neptune for Building a Graph Knowledge Base for GraphRAG
**Speaker:** Viet Phat

- **Traditional RAG vs. GraphRAG:** Plain RAG (vector database retrieval) struggles with complex relational data and multi-hop reasoning queries.
- **The GraphRAG Model:** Combining semantic searches with Graph Databases to map knowledge structures as entities and relationships.
- **Constructing Graph Knowledge Bases on AWS Neptune:** Using AWS Neptune as a fully managed graph database to store massive knowledge graphs. Running Gremlin or openCypher queries to fetch deep contextual data.
- **Impact:** Allowing Large Language Models (LLMs) to synthesize more accurate, deeper answers while explaining the logical connections behind data points.

#### 6. From IT Helpdesk to Senior Sysadmin: Self-Study Journey and Transition Roadmap
**Speaker:** Vinh Tran

- **Roles and Mindsets Shift:** Shifting from reactive user troubleshooting (IT Helpdesk) to proactive infrastructure planning and optimization (Sysadmin).
- **Required Skillsets for the Journey:**
  - *Networking & OS:* Deepening knowledge on TCP/IP, DNS, Linux administration (RedHat/Ubuntu), and Windows Server.
  - *Automation:* Writing automation scripts using Bash, PowerShell, or Python.
  - *Cloud & IaC:* Mastering cloud services (AWS, Azure) and Infrastructure as Code (Terraform).
- **Hands-on Self-Study Strategies:** Setting up a Home Lab using Proxmox, VMware, or AWS Free Tier for practice, and studying for industry-recognized certifications (CCNA, AWS SysOps, MCSA, Linux+).
- **Career Advice:** Remaining curious, welcoming difficult tasks in projects, and building systematic problem-solving habits.

---

### Key Takeaways

- **On Technical Knowledge:**
  - Mastered container packaging and multi-component system orchestration using Docker Compose.
  - Understood GraphRAG concepts and the critical role of AWS Neptune in improving AI query context and reasoning.
  - Learned how to integrate ML with AWS WAF for proactive defense, and deployment strategies for multiplayer game backends.
- **On Personal Growth:**
  - Acquired professional teamwork frameworks to work collaboratively and reduce team friction.
  - Formulated a clear self-study roadmap to build system administration competencies and advance my career.

### Applying to Work

- **Utilizing Docker:** Creating Dockerfiles and docker-compose files to package this internship report app and mock services, facilitating easier local testing and hosting.
- **Career Planning:** Constructing a weekly self-study roadmap focusing on Linux administration and automation scripting using Python.
- **Improving Collaboration:** Practicing clearer communication and strict code review processes when working on group projects or internship assignments.

### Event Experience

- An extremely valuable event covering diverse topics: basic infrastructure, network security, game development, and state-of-the-art AI integration (GraphRAG).
- Enthusiastic speaker presentations and live demos helped solidify complex theoretical concepts.
- The career advice session provided practical answers to burning questions faced by young IT engineers.

#### Some Event Photos
![FCAJ Tech Sharing Event](/images/4-EventParticipated/event2-photo.jpg)

> Overall, Demo Day 2 equipped me with sharp technical perspectives and strong motivation to continue refining both my hard and soft skills during my internship.
