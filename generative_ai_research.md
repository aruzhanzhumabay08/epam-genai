# Research on Generative AI Applications

Aruzhan Zhumabay
EPAM Tech Orda — GenAI for Software Development

## Why choose these cases

I'm new to this field, so for this report I looked at where generative AI is actually being used today, not just the theory. I focused on six areas that kept coming up while I was reading. For each one I tried to understand what problem it solves, what makes it hard to build, where it still falls short, and which real products already do it.

## 1. Coding assistants

A coding assistant lives inside the programmer's editor and suggests code as they type, or writes whole functions from English description. The appeal is obvious: it removes a lot of boring and repetitive typing and helps beginners get unstuck.

Where it gets tricky is context — the tool has to understand a big existing project to give useful suggestions. And the main weakness is trust, because the suggested code can look perfectly fine but be wrong or insecure, so you still have to read and check everything yourself.

Real products:
- GitHub Copilot — https://github.com/features/copilot — suggests code and functions right inside the editor.
- Cursor — https://cursor.com — a code editor built around AI chat that knows your whole project.
- Amazon Q Developer — https://aws.amazon.com/q/developer/ — AWS's assistant for writing and debugging code.

## 2. Customer support bots

Most of us have chatted with a support bot. The new generation runs on language models, so instead of only matching keywords, they actually understand different ways of asking the same thing and pull answers from the company's own help pages. For a business this means support around the clock and lower costs, while human agents handle the hard cases.

The catch is accuracy. If the bot gives a wrong or outdated answer confidently, it frustrates customers more than no bot at all. And it still struggles with very specific account problems.

Real products:
- Intercom Fin — https://www.intercom.com/fin — answers customer questions from a company's help content.
- Zendesk AI — https://www.zendesk.com/service/ai/ — AI built into Zendesk's support platform.
- Ada — https://www.ada.cx — automates customer service conversations.

## 3. Searching company knowledge (RAG)

Big companies have thousands of internal documents nobody can read through. RAG lets an employee just ask a question — the system finds the right internal documents, then the model answers using them. So you can basically chat with the company's own files.

It only works as well as the search behind it, if the wrong documents get pulled, the answer is weak. Keeping private data secure is also a big concern here.

Real products:
- Glean — https://www.glean.com — searches across all of a company's apps and documents.
- Microsoft 365 Copilot — https://www.microsoft.com/microsoft-365/copilot — answers using your company's files inside Office.
- Notion AI — https://www.notion.so/product/ai — answers questions from a team's Notion workspace.

## 4. Writing and marketing content

GenAI can draft blog posts, product descriptions, ads, and social media captions. A person sets the goal and tone, the model produces a first draft, and the human edits it. It saves time and makes it cheap to try many versions.

The honest downside is that the output often sounds generic, and it can state things that aren't true.

Real products:
- Jasper — https://www.jasper.ai — generates on-brand marketing content.
- Copy.ai — https://www.copy.ai — writes sales and marketing copy.
- Canva Magic Studio — https://www.canva.com/magic-studio/ — AI design and text tools inside Canva.

## 5. Summarizing long documents

Lawyers, analysts, and researchers read enormous documents. GenAI can summarize a long contract or report in seconds and answer specific questions about it. That saves hours.

But in serious fields like law or finance, a summary that quietly drops an important detail can be expensive, so people can't fully rely on it yet.

Real products:
- Harvey — https://www.harvey.ai — a GenAI assistant built for legal work.
- Hebbia — https://www.hebbia.com — analyzes large sets of financial documents.
- ChatPDF — https://www.chatpdf.com — lets you ask questions about any uploaded PDF.

## 6. AI agents

This is the most advanced one. Instead of answering a single question, an "agent" plans and carries out a task across several steps — it can create files, run code, call other tools, and report back with little supervision. Our course even mentions building one on EPAM's own platform.

The problem is reliability, over many steps there are many chances to make a mistake, and an agent with real access to systems can cause real damage if it goes wrong. These are harder to trust than a simple chatbot.

Real products:
- CodeMie — https://codemie.lab.epam.com — EPAM's platform for building AI agents and workflows.
- LangChain — https://www.langchain.com — a framework for building LLM apps and agents.
- Zapier AI — https://zapier.com/ai — automates tasks across many connected apps.

## What I took away

The pattern is pretty clear: generative AI speeds up anything that involves language, code, or content. The repeating risks are also clear — it can make things up, private data has to be protected, and people can start trusting it too much. So the real skill is knowing when to double-check it.
