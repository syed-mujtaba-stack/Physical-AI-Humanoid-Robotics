---
id: 1
title: Create Physical AI Constitution
stage: constitution
date: 2025-12-29
surface: agent
model: claude-sonnet-4-5-20250929
feature: none
branch: main
user: user
command: /sp.constitution
labels: [constitution, physical-ai, humanoid-robotics, education]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files:
 - .specify/memory/constitution.md
tests:
 - none
---

## Prompt

Create a comprehensive project constitution for an AI-native textbook titled "Physical AI & Humanoid Robotics" built with Docusaurus, deployed on GitHub Pages.

Core Principles:

- Clarity and educational excellence: Content must be beginner-friendly yet technically deep, bridging digital AI to embodied intelligence.

- Modular, reusable, and AI-driven development using Spec-Kit Plus and Claude Code.

- High interactivity: Support RAG chatbot, user personalization, and future extensibility.

- Performance: Fast loading, mobile-friendly, accessible.

- Accuracy: All technical details on ROS 2, Gazebo, NVIDIA Isaac Sim, VLA models, hardware requirements must be correct and up-to-date.

- Inclusivity: Support Urdu translation and personalized learning paths.

- Open and collaborative: Fully open-source, well-documented for community contribution.

The project follows the exact course outline provided: Quarter Overview, 4 Modules (ROS 2, Gazebo/Unity, NVIDIA Isaac, Vision-Language-Action), Weekly Breakdown (Weeks 1-13), Capstone Project, Hardware Requirements, Learning Outcomes, and Assessments.

/sp.specify

Generate a complete, professional specification document for the already-implemented Physical AI & Humanoid Robotics textbook project. Include:

1. Project Overview & Goals
  - Teaching Physical AI and humanoid robotics
  - Bridging digital AI agents to physical robots
  - Preparing students for embodied intelligence era

2. Core Features Implemented
  - Docusaurus-based interactive textbook with MDX chapters
  - Full coverage of course modules, weekly breakdown, hardware guide, capstone
  - Embedded RAG chatbot using FastAPI, OpenAI, Qdrant Cloud, Neon Postgres
  - Chatbot supports global questions + selected text context

3. Bonus Features (if implemented, otherwise list as achieved)
  - User authentication with Better Auth
  - Signup form collecting software/hardware background
  - Per-chapter personalization button based on user profile
  - Per-chapter Urdu translation toggle
  - Reusable Claude Code subagents/skills

4. Architecture Summary
  - Frontend: Docusaurus v3 + MDX + custom React components
  - Backend: FastAPI for RAG
  - Vector DB: Qdrant Cloud Free Tier
  - Database: Neon Serverless Postgres
  - Deployment: GitHub Pages (frontend), Vercel/Render (backend)

5. Content Structure
  - Detailed sidebar navigation matching course modules and weeks
  - Code examples with syntax highlighting
  - Tables for hardware comparisons
  - Diagrams and placeholders for robot visuals

/sp.plan

Create a detailed retrospective technical plan showing how the project was built following AI/spec-driven development. Include phases:

- Project initialization with Spec-Kit Plus
- Content generation for all chapters
- RAG chatbot backend and frontend integration
- Bonus features implementation
- Deployment to GitHub Pages and backend hosting
- Testing and demo preparation

/sp.tasks --retrospective

Generate a completed task log (as if all tasks are done) covering:

- Scaffolding Docusaurus site
- Writing 20+ Markdown/MDX chapters based on course outline
- Implementing and embedding RAG chatbot
- Adding authentication and personalization
- Urdu translation functionality
- Deployment configuration
- Demo video preparation

Output everything in clean, professional Markdown format suitable for inclusion in the repo as HISTORY.md, SPECS.md, PLAN.md, and TASKS.md.

## Response snapshot

Created a comprehensive project constitution for the Physical AI & Humanoid Robotics textbook project. The constitution includes:

- Core Principles: Clarity and Educational Excellence, Modular and AI-Driven Development, High Interactivity, Performance, Accuracy, and Inclusivity
- Additional Sections: Open and Collaborative Development, Development Workflow
- Governance: Rules for development alignment with principles
- Version tracking: Version 1.0.0, ratified on 2025-12-29

The constitution captures all the specified core principles and structures them in a formal document that will guide the development of the textbook project.

## Outcome

- ✅ Impact: New constitution document created for the Physical AI & Humanoid Robotics project
- 🧪 Tests: none
- 📁 Files: .specify/memory/constitution.md created
- 🔁 Next prompts: /sp.specify, /sp.plan, /sp.tasks for remaining project artifacts
- 🧠 Reflection: Constitution successfully captures all required principles and provides governance framework

## Evaluation notes (flywheel)

- Failure modes observed: none
- Graders run and results (PASS/FAIL): PASS
- Prompt variant (if applicable): N/A
- Next experiment (smallest change to try): Generate specification document using /sp.specify