# SecureMeBuddy - Showcase

# SecureMeBuddy

SecureMeBuddy is a web app designed to help people quickly check whether something online is safe or not.

Note: Some implementation details are intentionally kept private because this project is still evolving and includes backend logic and security-related workflows that are not part of the public showcase.

It gives users simple tools to analyze suspicious links, phone numbers, emails, and messages without needing technical knowledge.

## Live Site
https://securemebuddy.com

## What it does
- Check URLs for potential risks
- Analyze phone numbers and emails
- Help identify scam patterns and suspicious activity
- Provide simple, easy-to-understand safety feedback

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

    C --> H[SecureMeBuddy API Layer]
    D --> H
    E --> H
    F --> H

    H --> I[Supabase Edge Functions]
    I --> J[Supabase Database]

    I --> K[External Threat Intelligence APIs]
    K --> I

    J --> L[Scans]
    J --> M[Change Logs]
    J --> N[Reports / Alerts]

    H --> O[Risk Results Returned to Frontend]
    O --> B
This project is actively being developed and expanded.

---


