---
title: "PROPS – AI-Powered Obsolete Parts Search System"
excerpt: "Industry Capstone with B. Braun Medical Inc.<br/><br/>Built a secure, AI-powered web platform that automates sourcing of obsolete manufacturing parts across external marketplaces, reducing manual search time and production downtime for medical device engineers.<br/><br/><b>Tech:</b> Next.js, React, Tailwind CSS, OpenAI API (Web Search), JWT Auth<br/><b>Focus:</b> AI for supply chain, procurement automation, decision-support systems<br/><br/><img src='/images/222.png' style='width:20%; margin-right:10px;'><img src='/images/444.png' style='width:35%; margin-right:10px;'><img src='/images/333.png' style='width:35%;'>"
collection: portfolio
---

## Project Overview

PROPS (Potential Replacements for Obsolete Parts Search) is an AI-powered web application developed in collaboration with **B. Braun Medical Inc.**, a global leader in medical device manufacturing. The system addresses a critical supply-chain problem: locating replacement parts for obsolete or end-of-life manufacturing equipment.

Before PROPS, engineers manually searched multiple vendor websites, catalogs, and distributors — a process that could take weeks or months, causing extended equipment downtime and production delays. PROPS transforms this workflow into a single, AI-driven search experience.

## Problem Statement

- Manufacturing equipment relies on legacy and specialized components that frequently become obsolete
- Manual sourcing is time-consuming, inconsistent, and highly dependent on individual experience
- Extended downtime leads to missed production targets, increased operational risk, and delays in medical product delivery

B. Braun needed a secure, scalable, and intuitive system to modernize obsolete-part sourcing without automating final procurement decisions.

## Solution

We designed and implemented a web-based AI sourcing tool that allows engineers to:

- Input known part identifiers (manufacturer, part number, description, vendor)
- Trigger an AI-powered web search across multiple marketplaces
- Receive ranked replacement recommendations with:
  - Vendor links
  - Pricing & availability (when available)
  - Confidence score (1–100)
  - Natural-language justification

The system acts as a decision-support tool, not an automated buyer — preserving engineering oversight and compliance requirements.

## Key Features

- AI-powered web search using OpenAI (ChatGPT o4-mini with Web Search)
- Search-engine-style UI for fast adoption by engineers
- Structured JSON outputs for consistent rendering
- Confidence scoring & explanations for transparency
- Mobile-responsive design (validated via on-site factory visit)
- JWT-based authentication with enterprise-ready OAuth extensibility
- No data persistence (privacy-first, IT-compliant design)

## System Architecture

**Frontend:** React + Next.js, Tailwind CSS, Responsive component-based UI

**Backend:** Next.js API routes, OpenAI API integration, Secure JWT authentication (NextAuth)

**AI Layer:** OpenAI ChatGPT o4-mini, Real-time web search, JSON-formatted result ranking

**Security:** HTTPS for all requests, No exposed API keys, No storage of user or part data

## Engineering & Design Decisions

- Chose Next.js for full-stack simplicity and scalability
- Used LLM web search instead of scraping or licensed databases to avoid IP and compliance risks
- Ranked results instead of returning a single "best" answer to reduce false confidence
- Designed UI after familiar search engines (Google / Octopart) to minimize training time
- Optimized AI usage to keep token cost under $50

## Impact & Outcomes

- Reduced obsolete-part search time from days/weeks → minutes
- Centralized sourcing intelligence into one interface
- Improved engineering efficiency and reduced downtime risk
- Delivered a deployable prototype aligned with enterprise IT policies
- Validated through weekly sponsor reviews, factory floor site visit (Bethlehem, PA), and iterative demos

## My Role

**Software Engineer / AI Systems Developer**

- Designed AI prompting and result ranking logic
- Implemented frontend search & results UI
- Integrated OpenAI Web Search API
- Contributed to system architecture & security design
- Participated in stakeholder interviews and on-site user research
