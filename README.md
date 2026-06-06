# -ai-research-automation-pipeline

AI Research Article Automation Pipeline

Overview

This project is an automated end-to-end pipeline that transforms user-submitted topics into structured research articles using AI, dynamic data processing, and multi-platform integration.
It is currently a prototype (MVP stage) designed to validate system orchestration across multiple services and identify production-level improvements.
 
⸻
 
System Architecture
Flow:

Tally Form → Google Sheets → OpenAI (GPT-5.2) → JSON Parser → Pixabay API → Google Docs → Telegram Notification
 
⸻
 
Tech Stack

* Tally Forms (Input Layer)
* Google Sheets (Data Storage)
* OpenAI (GPT-5.2) (Content Generation)
* JSON Processing Engine
* Pixabay API (Image Retrieval)
* Google Docs API (Document Generation)
* Telegram Bot API (Notifications) 
⸻
 
Prompt Structure

AI generates structured JSON research articles:

* Title
* Introduction
* Sections (Heading + Content + Image Query)
* Conclusion
Strict formatting rules ensure valid RFC8259 JSON output.
 
⸻
 
Features

* Automated research article generation
* Structured JSON-based AI output
* Image integration via Pixabay API
* Automated Google Docs creation
* Telegram approval/revision system
* Multi-document output handling (large content splitting)
 
⸻
 
Current Limitations (MVP Stage)

1. Missing Headers/Subheaders

Issue: Flat document structure 
Fix: Enforce hierarchical mapping in prompt + Google Docs formatting layer
 
⸻
 
2. Image Spacing Issues

Issue: Images are tightly coupled with text 
Fix: Insert spacing paragraphs + apply Google Docs styling rules
 
⸻
 
3. Excessive Document Splitting

Issue: Output split into multiple documents (up to 8) 
Fix: Introduce batching logic and threshold-based pagination
 
⸻
 
Project Status

This is a test-stage automation system built to:

* Validate multi-service integration reliability
* Stress-test AI-generated structured outputs
* Identify scalability bottlenecks
* Provide foundation for a production-grade pipeline system

Future iterations will focus on:

* Output consolidation
* Advanced formatting engine
* Error recovery system
* Scalable document orchestration layer
 
⸻
 
Setup (Future Improvement Placeholder)

Full setup instructions will be added once production version is finalized.
 
⸻
 
Output Example

* Automated research article
* Structured Google Doc
* Embedded images
* Telegram approval workflow
 
⸻
 
Author Intent

This project serves as a foundational architecture for a scalable AI-driven content pipeline system capable of generating structured, multi-modal research outputs at scale.
