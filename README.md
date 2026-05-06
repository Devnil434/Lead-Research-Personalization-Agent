# AI Lead Intelligence & Outreach Agent

An AI-powered no-code/low-code lead research and outreach automation system built using n8n, OpenAI APIs, JavaScript, and Google Sheets.

The workflow automatically researches companies, analyzes their websites using AI, scores lead quality, identifies growth opportunities, and generates personalized outreach messages at scale.

---

# Demo

## Loom Walkthrough
(Add Loom link here)

---

# Problem

Sales and growth teams spend significant time:
- researching company websites,
- understanding business positioning,
- qualifying leads,
- identifying opportunities,
- and writing personalized outreach manually.

This process is repetitive, time-consuming, and difficult to scale.

---

# Solution

This workflow automates the entire lead intelligence pipeline.

The agent:
1. accepts company URLs,
2. fetches website content,
3. cleans raw HTML,
4. analyzes businesses using AI,
5. generates structured lead intelligence,
6. creates personalized outreach,
7. and exports results into Google Sheets automatically.

---

# Features

## AI Company Analysis
Automatically extracts:
- company summary
- industry
- company type
- competitors
- growth opportunities
- business positioning

---

## Lead Qualification
Generates:
- lead score
- fit score
- confidence score

---

## Personalized Outreach
Creates:
- personalized email subject lines
- outreach messages
- growth-focused personalization

---

## Google Sheets CRM Export
Automatically stores structured lead intelligence into Google Sheets.

---

## Production-Style Edge Cases
Handles:
- invalid URLs
- website fetch failures
- malformed AI JSON
- low-content websites
- retry handling
- duplicate companies
- partial failures without crashing workflow

---

# Tech Stack

- n8n
- OpenAI API
- JavaScript
- Google Sheets API
- HTTP Request Nodes
- JSON Parsing Workflows

---

# Architecture

```text
Company Input
      ↓
URL Validation
      ↓
Website Fetching
      ↓
HTML Cleaning
      ↓
OpenAI Analysis
      ↓
JSON Parsing & Repair
      ↓
Lead Scoring
      ↓
Outreach Generation
      ↓
Google Sheets Export
