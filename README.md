<div align="center">

# Skand Shukla

**Backend Developer · Cloud & Infrastructure · Security Engineering**

Delhi, India &nbsp;|&nbsp; [GitHub](https://github.com/Skand203) &nbsp;|&nbsp; [Email](mailto:skandshukla2004@gmail.com) &nbsp;|&nbsp; [LinkedIn](https://linkedin.com/in/)

</div>

---

### 👨‍💻 About Me

I am a Computer Science and Engineering undergraduate focused on building robust backend systems, reliable cloud infrastructure, and practical security software.

- **Systems-first mindset:** I prefer learning through building from scratch—understanding how protocols, operating thresholds, and cloud services behave under real-world conditions rather than treating them as black boxes.
- **Backend & Cloud:** Experienced with Python and TypeScript backends, RESTful API design, and event-driven serverless architectures on Amazon Web Services (AWS).
- **Security Engineering Interest:** Engaged in network intrusion anomaly detection, threshold calibration transfer research, and security telemetry analysis.
- **Goal:** Seeking a backend / software engineering role where I can contribute to production-grade services, API design, and scalable infrastructure.

---

### 🛠️ Tech Stack

#### Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)

#### Backend & APIs
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js%20API%20Routes-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST-Architecture-blue?style=flat-square)
![Event-Driven](https://img.shields.io/badge/Event--Driven-Architecture-blueviolet?style=flat-square)

#### Cloud & Infrastructure
![AWS Lambda](https://img.shields.io/badge/AWS%20Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![Amazon DynamoDB](https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)
![Amazon API Gateway](https://img.shields.io/badge/Amazon%20API%20Gateway-FF4F8B?style=flat-square&logo=amazonapigateway&logoColor=white)
![AWS IAM](https://img.shields.io/badge/AWS%20IAM-DD344C?style=flat-square&logo=amazoniam&logoColor=white)
![CloudWatch](https://img.shields.io/badge/Amazon%20CloudWatch-FF4F8B?style=flat-square&logo=amazoncloudwatch&logoColor=white)

#### Databases & Storage
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Amazon DynamoDB](https://img.shields.io/badge/DynamoDB-NoSQL-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-Object%20Store-569A31?style=flat-square&logo=amazons3&logoColor=white)

#### Security & Systems Engineering
![Network Anomaly Detection](https://img.shields.io/badge/NIDS-Anomaly%20Detection-critical?style=flat-square)
![Statistical Calibration](https://img.shields.io/badge/Calibration-Quantile%20Transfer-informational?style=flat-square)
![Security Telemetry](https://img.shields.io/badge/Security-Log%20Ingestion%20%26%20Telemetry-darkgreen?style=flat-square)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

#### Developer Tools
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)

---

### 🚀 Featured Projects

#### [CloudDrop](https://github.com/Skand203/CloudDrop)
**Serverless File Storage & Management Platform (AWS)**
- **Problem:** Conventional file uploads routed through monolithic web servers create bandwidth bottlenecks, CPU saturation, and unnecessary server idle costs.
- **Solution:** Designed and deployed a fully serverless, event-driven file storage service using AWS Lambda, API Gateway, Amazon S3, and Amazon DynamoDB.
- **Technical Highlights:**
  - Implemented pre-signed URL generation via `boto3` Lambda to offload heavy binary file streams directly to Amazon S3 with an ephemeral 300-second TTL.
  - Configured S3 `ObjectCreated` event notifications to asynchronously trigger metadata extraction and index object sizes, UUID keys, and timestamps in DynamoDB.
  - Implemented a unified `FileManager` Lambda managing file listings, secure download redirects, and atomic deletions across both storage and database tiers.
- **Tech Stack:** Python, AWS Lambda, Amazon S3, Amazon DynamoDB, Amazon API Gateway, AWS IAM, JavaScript.

---

#### [benign-calibrated-nids](https://github.com/Skand203/benign-calibrated-nids)
**Empirical Evaluation of Calibration Transfer in Network Anomaly Detection**
- **Problem:** Benchmark evaluations of network intrusion detection systems (NIDS) routinely rely on threshold-independent metrics (e.g., ROC-AUC) or unrealistic "oracle" test-set tuning, obscuring how severely false-positive rates explode when deployed on unseen traffic.
- **Solution:** Authored a complete, reproducible empirical research codebase evaluating Isolation Forests, Local Outlier Factor (LOF), and One-Class SVM on 257,673 records from the UNSW-NB15 benchmark.
- **Technical Highlights:**
  - Implemented multi-seed label-blind quantile calibration pipelines on benign traffic to enforce strict operational false-positive budgets ($\alpha = 1\%, 3\%, 5\%$).
  - Quantified calibration transfer divergence and uncovered structural benchmark distortions caused by categorical vocabulary mismatch and duplicated flow vectors.
  - Packaged the full pipeline with reproducible notebooks, diagnostic audits, statistical summaries, and publication-ready figures.
- **Tech Stack:** Python 3.11, scikit-learn, NumPy, Pandas, Matplotlib, Jupyter, UNSW-NB15 Benchmark.

---

#### [BigQuery Release Radar](https://github.com/Skand203/BigQuery-Release-Radar)
**Structured Cloud Feed Parser & Digest Generator**
- **Problem:** Google Cloud BigQuery bundles frequent product updates into monolithic daily Atom/XML entries, making it difficult for data engineers and cloud practitioners to track, filter, and share individual feature updates or deprecations.
- **Solution:** Built a Python Flask web application that continuously fetches the official BigQuery release RSS feed, parses unstructured CDATA HTML into distinct typed updates (Features, Fixes, Changes, Notices), and enables real-time search, categorization, and tweet compilation.
- **Technical Highlights:**
  - Developed custom DOM traversal algorithms with BeautifulSoup to cleanly segment composite daily entries into structured event cards.
  - Built an interactive Twitter digest composer that dynamically tracks tweet character limits while accurately budgeting 23 characters for Twitter `t.co` URL wrapping.
  - Included unit test coverage (`test_parser.py`) validating feed parsing, HTML sanitization, and fallback behavior across varying feed schemas.
- **Tech Stack:** Python, Flask, BeautifulSoup4, feedparser, JavaScript, HTML5/CSS3.

---

#### [SafeSathi AI](https://github.com/Skand203/SafeSathi-AI)
**Bilingual Scam Detection Platform for Senior Citizens**
- **Problem:** Digital financial fraud in India disproportionately impacts senior citizens through deceptive WhatsApp forwards, fake KYC urgencies, and fraudulent APK downloads, while existing security tools rely on dense English security terminology.
- **Solution:** Developed an accessible, bilingual (English & Hindi) fraud analysis platform submitted for the Google Solution Challenge 2026 (supporting UN SDG 16).
- **Technical Highlights:**
  - Built a serverless API endpoint in Next.js that validates input bounds and prompts Google Gemini Flash to identify psychological urgency, malicious URLs, and OTP extraction patterns.
  - Structured risk outputs into strict JSON schemas (`Safe`, `Suspicious`, `High Danger`) paired with empathetic, non-technical guidance.
  - Implemented native browser Web Speech API synthesis (`SpeechSynthesis`) for one-tap voice readouts in Hindi (`hi-IN`) and English (`en-US`), paired with WCAG AA compliant high-contrast UI.
- **Tech Stack:** Next.js 16 (App Router), TypeScript, Google Gemini API, Tailwind CSS, Web Speech API.

---

#### [AI-Assisted Security Operations Center](https://github.com/Skand203/AI---Assisted-Security-Operations-Center)
**Foundational Telemetry & Event Ingestion Engine (In Development)**
- **Problem:** Security teams experience severe alert fatigue from fragmented log streams and manual rule triage.
- **Solution:** Early-stage open-source security operations center backend designed to ingest endpoint telemetry, correlate security events against deterministic detection rules, and provide automated investigation summaries.
- **Current Progress:** Foundational FastAPI service architecture, endpoint health-check contracts, and development branch structure establishing the log ingestion pipeline.
- **Tech Stack:** Python, FastAPI, PostgreSQL, Git workflow.

---

#### [CyberSentinel](https://github.com/Skand203/CyberSentinel)
**Evidence-Driven Suspicious Content Analysis Engine (Architecture & Design)**
- **Focus:** System design and specification for a multi-stage security analysis platform to analyze URLs, email headers, and messages for deception indicators through static extraction, threat reputation APIs, and structured evidence reports.
- **Status:** Architectural blueprint, data schema definition, and pipeline design.

---

### 🔍 Currently Exploring

- **Distributed Systems & Asynchronous Pipelines:** Implementing message brokers (RabbitMQ / Apache Kafka) for decoupled event processing.
- **Containerization & Deployment:** Packaging multi-container services with Docker and automating CI/CD workflows via GitHub Actions.
- **API Security Hardening:** Implementing rate-limiting algorithms (token bucket / leaky bucket) and robust OAuth2/JWT authentication workflows.

---

### 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Skand203&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&icon_color=58a6ff" alt="Skand Shukla's GitHub Stats" width="48%" />
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Skand203&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9" alt="Top Languages" width="44%" />

</div>

---

### 📬 Connect with Me

- **Email:** [skandshukla2004@gmail.com](mailto:skandshukla2004@gmail.com)
- **GitHub:** [github.com/Skand203](https://github.com/Skand203)
- **LinkedIn:** [linkedin.com/in/](https://linkedin.com/in/)

---
<div align="center">
<sub>Designed with a focus on systems engineering, clean architecture, and practical software development.</sub>
</div>
