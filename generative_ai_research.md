# Research Report: Generative AI Applications

**Author:** Aruzhan Zhumabay
**Program:** EPAM Tech Orda — Generative AI for Software Development
**Module:** Introduction

---

## Introduction

Generative AI (GenAI) refers to a class of artificial intelligence systems that create new content — text, code, images, audio, or structured data — rather than only classifying or predicting from existing data. Most modern GenAI systems are built on large language models (LLMs) trained on very large datasets. This report surveys several real-world application areas, describing for each the business value it creates, the main technical challenges, its weak points, and existing implementations.

---

## 1. AI-Assisted Software Development (Code Generation)

AI coding assistants suggest, complete, and generate source code directly inside a developer's editor. A developer describes what they want in natural language or starts typing, and the model proposes the next lines, whole functions, or tests. This use case is central to the software industry because it directly shortens the time between an idea and working code.

**Business value:** Faster development, fewer repetitive tasks, lower onboarding time for junior developers, and more consistent code. Studies by vendors report meaningful productivity gains on routine coding tasks. **Technical challenges:** Keeping suggestions correct and secure, giving the model enough context about a large codebase, and integrating smoothly into existing tools. **Weak points:** The model can produce confident but wrong or insecure code ("hallucinations"), may leak patterns from training data, and can make developers over-rely on suggestions without understanding them.

**Existing implementations:**
- **GitHub Copilot** — https://github.com/features/copilot — An AI pair programmer that suggests code and whole functions inside the editor.
- **Amazon Q Developer** — https://aws.amazon.com/q/developer/ — AWS's assistant for writing, testing, and debugging code.
- **Cursor** — https://cursor.com — An AI-first code editor built around chat and codebase-aware editing.

---

## 2. Customer Support Assistants (Chatbots)

GenAI chatbots answer customer questions in natural language, resolve common issues, and escalate harder cases to human agents. Unlike older rule-based bots, LLM-based assistants understand varied phrasing and can hold a coherent conversation, often pulling answers from a company's own documentation.

**Business value:** Lower support costs, 24/7 availability, faster response times, and freeing human agents for complex problems. **Technical challenges:** Grounding answers in accurate company data, handling many languages, and keeping responses on-topic and safe. **Weak points:** Risk of giving wrong or outdated answers, difficulty with highly specific account issues, and customer frustration when the bot cannot escalate properly.

**Existing implementations:**
- **Intercom Fin** — https://www.intercom.com/fin — An AI support agent that resolves customer questions using a company's help content.
- **Zendesk AI** — https://www.zendesk.com/service/ai/ — AI features built into Zendesk's customer service platform.
- **Ada** — https://www.ada.cx — An AI-powered customer service automation platform.

---

## 3. Enterprise Knowledge Assistants (RAG)

Retrieval-Augmented Generation (RAG) combines an LLM with a company's private documents. When a user asks a question, the system first retrieves the most relevant internal documents and then asks the model to answer using them. This lets employees "chat" with company knowledge — policies, manuals, reports — without reading everything manually.

**Business value:** Faster access to internal knowledge, reduced time spent searching, and better decisions based on current company data. **Technical challenges:** Building a good search/retrieval layer, keeping documents up to date, and controlling who can access which data. **Weak points:** If retrieval returns poor documents, the answer is weak; models can still hallucinate; and sensitive data must be carefully protected.

**Existing implementations:**
- **Glean** — https://www.glean.com — An AI-powered work assistant that searches across a company's apps and documents.
- **Microsoft 365 Copilot** — https://www.microsoft.com/microsoft-365/copilot — An assistant integrated into Office apps that answers using company data.
- **Notion AI** — https://www.notion.so/product/ai — AI features that answer questions and generate content from a team's Notion workspace.

---

## 4. Content Creation and Marketing

GenAI generates marketing copy, blog posts, product descriptions, social media content, and images. Marketers describe the goal, tone, and audience, and the model drafts content that a human then reviews and edits.

**Business value:** Faster content production, lower cost per asset, easy personalization and localization, and more creative options to test. **Technical challenges:** Keeping brand voice consistent, avoiding factual errors, and generating truly original rather than generic content. **Weak points:** Output can feel generic or repetitive, may contain mistakes, and raises copyright and originality concerns.

**Existing implementations:**
- **Jasper** — https://www.jasper.ai — A marketing-focused platform for generating on-brand content.
- **Copy.ai** — https://www.copy.ai — A tool for generating marketing and sales copy.
- **Canva Magic Studio** — https://www.canva.com/magic-studio/ — AI design and content tools inside Canva.

---

## 5. Document Summarization and Analysis

GenAI reads long documents — contracts, reports, research papers, meeting transcripts — and produces short summaries, extracts key points, or answers specific questions about them. This is valuable in law, finance, research, and any field with heavy reading.

**Business value:** Saves professionals hours of reading, surfaces key information quickly, and makes large document sets usable. **Technical challenges:** Handling very long documents, staying accurate on critical details, and processing different file formats. **Weak points:** Summaries can miss or distort important nuances, and errors in high-stakes documents (legal, medical) can be costly.

**Existing implementations:**
- **Harvey** — https://www.harvey.ai — A GenAI assistant built for legal work and document analysis.
- **Hebbia** — https://www.hebbia.com — An AI platform for analyzing large sets of financial and business documents.
- **ChatPDF** — https://www.chatpdf.com — A simple tool to ask questions about an uploaded PDF.

---

## 6. AI Agents and Workflow Automation

AI agents go beyond single answers: they plan and carry out multi-step tasks by calling tools, APIs, and other systems. For example, an agent might read a task, create files, run code, and report results — with limited human supervision.

**Business value:** Automates complex, multi-step work, reduces manual effort, and can operate continuously. **Technical challenges:** Reliability over many steps, safe access to real systems, and recovering from mistakes without human help. **Weak points:** Agents can fail or loop on complex tasks, take wrong actions if poorly constrained, and are harder to test and trust than simple assistants.

**Existing implementations:**
- **CodeMie** — https://codemie.lab.epam.com — EPAM's platform for building and running AI agents and workflows.
- **LangChain / LangGraph** — https://www.langchain.com — A framework for building applications and agents powered by LLMs.
- **Zapier AI** — https://zapier.com/ai — AI-driven automation across thousands of connected apps.

---

## Conclusion

Generative AI is already delivering real value across software development, customer service, knowledge management, marketing, document analysis, and automation. The common pattern is clear: GenAI accelerates work that involves language, code, or content. The common risks are also clear — hallucinations, data privacy, and over-reliance. Successful adoption depends not only on the models themselves but on grounding them in reliable data, keeping humans in the loop, and carefully handling security and accuracy.
