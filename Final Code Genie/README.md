**CodeGenie – AI Code Generator & Explainer******
**Infosys Springboard Internship – Final Project**

🔮 Overview

CodeGenie is an AI-powered programming assistant designed to improve coding education, development workflows, and debugging efficiency.
It supports natural language to code, intelligent code explanation, AI chat assistance, secure authentication, and admin-level analytics.

This project integrates modern open-source LLMs, advanced security mechanisms, and interactive UI components for a complete learning + development ecosystem.

🧠 Key Features
1️⃣ AI Code Generator

Converts natural language descriptions into clean, executable code

Multi-language support: Python, JavaScript, Java, C++, SQL, Go, HTML, CSS, Rust

Supports:

Syntax-aware code generation

Context-based completion

Models used:

Gemma-2B-IT (Google) – fastest

DeepSeek-Coder-1.3B – well-balanced

Phi-2 – reliable general-purpose

CodeLlama-7B (Meta) – best accuracy

StarCoder2-3B – multi-language expert

2️⃣ AI Code Explainer

Provides detailed breakdown of any code snippet with:

High-level overview

Line-by-line explanation

Time & space complexity

Edge case identification

Optimization suggestions

Special features:

AST Visualization (Python)

Syntax highlighting

Logic flow diagrams

3️⃣ AI Chat Assistant

Interactive chat for debugging, guidance, and coding help

Maintains context over conversation

Learns from user prompts for improved responses

4️⃣ Conversation Management

Save, delete, and search all conversation history

Auto-generates conversation titles

Create shareable read-only links

Organize past interactions efficiently

5️⃣ User Authentication System

Secure JWT-based login system:

Access Token: 24-hour validity

Refresh Token: 7-day validity

Auto session refresh

Security Features:

BCRYPT password hashing

SQL injection protection

Session timeout

RBAC (Role-Based Access Control)

Users → code generation, explanation

Admins → full system access

Password Recovery:

Email-based OTP

Security questions

6️⃣ Admin Dashboard

Admin panel includes:

User promotion/demotion

Live system monitoring

Global activity logs

User analytics

Language usage metrics

Model performance charts

Rules:

Maximum 2 admins

First registered user becomes admin

Cannot delete last active admin

🏗️ System Architecture

Includes:

High-level architecture diagrams

Component-based system breakdown

ER diagram for DB schema

Secure request flow for JWT auth

Multi-model execution pipeline

(All diagrams included in the project presentation)

📊 Results & Evaluation
Model Performance

Gemma-2B-IT → Best speed (1.8s avg)

CodeLlama-7B → Best accuracy (92%)

DeepSeek-Coder → Best balance (89% accuracy, 3.1s)

User Engagement

Total Users: 15+

Conversations: 30+

Code Generations: 30+

Explanations: 30+

Feedback Rating: 4.1 / 5

Success Indicators

✔ Multi-language support
✔ Fast response times
✔ Secure authentication system
✔ High user satisfaction
✔ Comprehensive analytics

🧩 Challenges & Learnings
1. GPU Model Management

Problem: Memory constraints while loading multiple models

Solution: Dynamic loading & unloading

Learning: Efficient VRAM usage is crucial

2. Response Quality

Problem: Inconsistent output quality across models

Solution: Advanced prompt engineering

Learning: Prompt design heavily affects model performance

3. Real-Time Updates

Problem: Admin dashboard refresh overhead

Solution: Optimized SQL queries + 15s refresh cycle

🎯 Conclusion

CodeGenie transforms programming education by offering:

Smarter learning tools

Faster debugging workflows

Multi-model AI support

Secure and scalable user management

Insightful analytics and monitoring

It empowers students, educators, and developers with a next-generation AI coding ecosystem.
