# SecureMeBuddy - Showcase
> Simple tools for spotting scams and staying safe online.


SecureMeBuddy is a web app designed to help people quickly check whether something online is safe or not.

It provides simple tools to analyze suspicious links, phone numbers, and emails without requiring technical knowledge.

> Note: This repository is a public-facing showcase. Some implementation details are intentionally kept private as the project includes backend logic and security-focused workflows that are still evolving.

It gives users simple tools to analyze suspicious links, phone numbers, emails, and messages without needing technical knowledge.

## Live Site
https://securemebuddy.com

## What it does
- Check URLs for potential risks
- Analyze phone numbers and emails
- Help identify scam patterns and suspicious activity
- Provide simple, easy-to-understand safety feedback

## Admin Dashboard

A centralized operations console for monitoring platform activity, scan results, and system health.

### Operations Overview
<img src="https://github.com/user-attachments/assets/a696743f-c580-4707-a067-ead51d85fe98" width="100%" />

### Intelligence Center
<img src="https://github.com/user-attachments/assets/731840aa-1097-4c34-a9ea-bd04cde0f3c0" width="100%" />

### Signals & Activity
<img src="https://github.com/user-attachments/assets/38e9fb63-a2c9-490c-b170-706ea2bfce86" width="100%" />

### Change Log
<img src="https://github.com/user-attachments/assets/d43f03c8-886d-4956-a104-df72534a908b" width="100%" />

## Why I built this
Scams are getting more convincing, and most tools are either too technical or too hidden.

I wanted to build something that feels accessible — something anyone can use without needing to understand cybersecurity.

The goal is to make online safety tools easier, faster, and more approachable.

## Tech Stack
- Next.js
- React
- Supabase (backend + database)
- Edge Functions
- External threat intelligence APIs

## Key Features
- Real-time safety checks
- Dashboard with lookup tracking and stats
- Structured logging system for threat data
- Scalable backend using Supabase functions

## Project Direction
SecureMeBuddy is evolving beyond a simple checker tool into a broader safety platform.

Planned improvements include:
- Public threat feed
- Smarter risk scoring and classification
- Gamification (user reporting, rankings, badges)
- Improved analytics and data insights

## What I’ve learned
- Designing systems that balance usability with security
- Structuring backend services for real-time data processing
- Building with scalability in mind from early stages

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
