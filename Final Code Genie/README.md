**CodeGenie – AI Code Generator & Explainer**


**Infosys Springboard Internship – Final Project**

**🔮 Overview**

CodeGenie is an AI-powered programming assistant designed to enhance coding education, development workflows, and debugging efficiency.
It supports natural language → code, intelligent code explanation, AI chat, secure authentication, and admin-level analytics.

This project integrates modern open-source LLMs, advanced security mechanisms, and interactive UI components to deliver a complete AI-driven learning + development ecosystem.

**🧠 Key Features**

1️⃣ AI Code Generator

Converts natural language descriptions into clean, executable code

Multi-language support:
Python, JavaScript, Java, C++, SQL, Go, HTML, CSS, Rust

Supports:

Syntax-aware code generation

Context-based completion

Models Used:

Gemma-2B-IT (Google) – fastest

DeepSeek-Coder-1.3B – well-balanced

Phi-2 (Microsoft) – reliable general-purpose

CodeLlama-7B (Meta) – best accuracy

StarCoder2-3B – multi-language expert

2️⃣ AI Code Explainer

Provides advanced breakdown of any code snippet with:

High-level overview

Line-by-line explanation

Time & space complexity

Edge case identification

Optimization suggestions

Special Features:

AST Visualization (Python)

Syntax highlighting

Logic flow diagrams

3️⃣ AI Chat Assistant

Interactive AI chat for debugging and guidance

Maintains conversation context

Learns from user prompts for improved responses

4️⃣ Conversation Management

Save, delete, and search conversation history

Auto-generated conversation titles

Create shareable read-only links

Efficiently organize past sessions

5️⃣ User Authentication System

Secure JWT-based login system:

Access Token → 24-hour validity

Refresh Token → 7-day validity

Auto session refresh

Security Features:

BCRYPT password hashing

SQL injection protection

Session timeout

RBAC (Role-Based Access Control):

Users: code generation, explanation

Admins: full system access

Password Recovery Options:

Email-based OTP

Security questions

6️⃣ Admin Dashboard

Includes advanced admin functionalities:

User promotion/demotion

Live system monitoring

Global activity logs

User analytics

Language usage metrics

Model performance stats

Rules:

Maximum 2 admins

First registered user becomes admin

Cannot delete the last active admin

🏗️ System Architecture

Includes complete project documentation with:

High-level architecture diagrams

Component-based design

ER diagram (Database Schema)

Secure JWT authentication flow

Multi-model execution pipeline

(All diagrams are provided in the project presentation.)

📊 Results & Evaluation
Model Performance

Gemma-2B-IT: Best speed (1.8s avg)

CodeLlama-7B: Best accuracy (92%)

DeepSeek-Coder: Best balance (89% accuracy, 3.1s)

User Engagement

15+ Users

30+ Conversations

30+ Code Generations

30+ Explanations

4.1 / 5 Feedback Rating

Success Indicators

✔ Multi-language support
✔ Sub-5-second response time
✔ Secure authentication
✔ High user satisfaction
✔ Comprehensive analytics

🧩 Challenges & Learnings
1. GPU Model Management

Problem: Memory constraints while loading models

Solution: Dynamic loading & unloading

Learning: Efficient VRAM usage is critical

2. Response Quality

Problem: Inconsistent output quality across models

Solution: Advanced prompt engineering

Learning: Prompt design has a major impact on output

3. Real-Time Updates

Problem: Admin dashboard refresh load

Solution: Optimized SQL queries + 15-second refresh cycle

🎯 Conclusion

CodeGenie transforms programming education by providing:

Smarter AI-powered learning tools

Faster debugging workflows

Multi-model AI support

Secure & scalable user management

Insightful analytics and monitoring

It empowers students, educators, and developers with a robust next-generation AI coding ecosystem.
