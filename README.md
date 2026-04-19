# SecureMeBuddy – Showcase
> Simple tools for spotting scams and staying safe online.

SecureMeBuddy is a web app designed to help people quickly check whether something online is safe or not. It provides simple, accessible tools to analyze suspicious links, phone numbers, emails, and messages—without requiring technical knowledge.

As a registered business and actively developed platform, SecureMeBuddy is focused on making online safety tools more accessible and practical for everyday use.

> Note: This repository is a public-facing showcase. Some implementation details are intentionally kept private as the project includes backend logic and security-focused workflows that are still evolving.

---

## Live Site
https://securemebuddy.com

---

## What it does
- Check URLs for potential risks  
- Analyze phone numbers and emails  
- Identify scam patterns and suspicious activity  
- Provide clear, easy-to-understand safety feedback  

---

## Frontend / User Experience

### Homepage
<img width="938" height="988" src="https://github.com/user-attachments/assets/0f2e9736-a5b9-4c15-abad-9ed459636522" />

### Tools
<img width="933" height="986" src="https://github.com/user-attachments/assets/d6824156-9269-49e6-8d2e-f953c0c4b74c" />

### Community Reports
<img width="929" height="983" src="https://github.com/user-attachments/assets/4e6a9ce1-6a4e-44f8-8108-30b43efc1742" />

### Protection Picks
<img width="893" height="982" src="https://github.com/user-attachments/assets/41cc6c77-5e0d-4433-85b6-6821807eb452" />

### Learn Hub
<img width="838" height="987" src="https://github.com/user-attachments/assets/a2c6f163-5c22-4588-bc00-08edc61e0078" />

### Authentication
<img width="939" height="985" src="https://github.com/user-attachments/assets/1b232aac-9c15-4bce-af89-566adb4970ab" />

### User Dashboard
<img width="839" height="983" src="https://github.com/user-attachments/assets/9a1c3428-a84c-497b-bdd1-7ef83b75b2d0" />

### User Settings
<img width="837" height="983" src="https://github.com/user-attachments/assets/44127221-b426-4057-b8bd-f3bf532fbd6d" />

### Threat Reports
<img width="920" height="988" src="https://github.com/user-attachments/assets/168dd8a1-c33c-4959-b7ed-230bd6f47b3c" />

---

## Admin Dashboard

A centralized operations console for monitoring platform activity, scan results, and system health in real time.

### Operations Overview
<img src="https://github.com/user-attachments/assets/a696743f-c580-4707-a067-ead51d85fe98" width="100%" />

### Intelligence Center
<img src="https://github.com/user-attachments/assets/731840aa-1097-4c34-a9ea-bd04cde0f3c0" width="100%" />

### Signals & Activity
<img src="https://github.com/user-attachments/assets/38e9fb63-a2c9-490c-b170-706ea2bfce86" width="100%" />

### Change Log
<img src="https://github.com/user-attachments/assets/d43f03c8-886d-4956-a104-df72534a908b" width="100%" />

---

## Why I built this

Scams are becoming more convincing, while many security tools remain too technical or difficult to access.

I built SecureMeBuddy to make online safety tools simple, fast, and usable for everyday people—without requiring a background in cybersecurity.

---

## Tech Stack
- Next.js  
- React  
- Supabase (database + backend)  
- Edge Functions  
- External threat intelligence APIs  

---

## Key Features
- Real-time safety checks  
- Lookup tracking and activity dashboards  
- Structured logging system for threat data  
- Scalable backend using serverless functions  

---

## Project Direction

SecureMeBuddy is evolving beyond a simple checker into a broader security platform.

Planned improvements include:
- Public threat intelligence feed  
- Smarter risk scoring and classification  
- Gamification (user reports, rankings, badges)  
- Expanded analytics and insights  

---

## What I’ve learned
- Designing systems that balance usability with security  
- Structuring backend services for real-time processing  
- Building with scalability in mind from early stages  

---

## Architecture Overview

```mermaid
flowchart TD
    A[User] --> B[SecureMeBuddy Frontend]

    B --> C[URL Checker]
    B --> D[Email Checker]
    B --> E[Phone Checker]
    B --> F[Threat Reports]
    B --> G[Safety Center]

    C --> H[API Layer]
    D --> H
    E --> H
    F --> H

    H --> I[Supabase Edge Functions]
    I --> J[Supabase Database]

    I --> K[Threat Intelligence APIs]
    K --> I

    J --> L[Scans]
    J --> M[Change Logs]
    J --> N[Reports / Alerts]

    H --> O[Results]
    O --> B
