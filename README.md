# Rule Creator

Welcome to the **Rule Creator** repository, an AI-powered security rule management platform. This project helps create, analyze, and optimize detection rules across multiple security platforms.

This repository contains two primary modules/environments:

1. **DetectIQ**: 
   An AI-powered security rule management platform focused on generating, testing, and managing threat detection rules efficiently. It includes an interactive UI and Python module to automate security tasks utilizing OpenAI's LLMs. 
   
2. **Malware Analysis**: 
   A specialized environment based on DetectIQ designed for deep diving into static analysis. It supports uploading malware samples (like `.exe`) and `.pcap` files for automated analysis, automatically mapping context to YARA and Snort rule creation.

## Key Features
- **AI-Powered Detection Engine**: Rapidly generate custom Sigma, YARA, and Snort rules using LLMs contextually aware of existing platforms.
- **Rule Repository Integration**: Integrates directly with standard rule repositories (SigmaHQ, YARA-Forge, Snort3 Community).
- **Static Analysis**: Extract details automatically from pcap or malware samples.
- **Multi-Platform Integration**: Automate the translation of conceptual rules (Sigma) to specific SIEM queries (Splunk, etc.) using `pySigma`.

## Getting Started

Each module contains its own documentation. To get started, navigate to the module of your choice:

```bash
# To start with DetectIQ
cd DetectIQ
bash start.sh install
bash start.sh run

# To start with Malware Analysis
cd "Malware Analysis"
bash start.sh install
bash start.sh run
```

Then visit [http://localhost:3000](http://localhost:3000) in your web browser.

> **Disclaimer**: This tool is an active Proof of Concept. Treat with care and do not deploy in sensitive production environments without proper validation!

## License
Refer to the individual modules for detailed licensing, generally falling under LGPL v2.1 (core), DRL (Sigma), YARAForge, and GPL with VRT (Snort).
