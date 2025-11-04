# 300 Days Of Code - Year 2 🚀

Welcome back to my coding journey!

This repository marks the second year of my 300 Days of Code challenge.

Last year focused heavily on daily logs and updates within the realm of vision technologies. This year, the focus shifts towards deeper dives into key bootcamps and substantial projects, moving away from daily standup-style logging.

The goal remains consistent: dedicated coding effort. However, the definition of a "minimum viable day" is now centered on completing the LeetCode daily challenge. This ensures consistent problem-solving practice while allowing for more flexibility to concentrate on larger learning modules and projects.

_This repo links out to submodules and folders containing detailed work and documentation._

---

## Challenge Structure

- **LeetCode**: Daily challenges (code in `/leetcode/`, certificates in `/certs/leetcode/`)
- **Bootcamps**: Each bootcamp tracked as a submodule
- **Projects**: Larger projects get their own folders
- **Milestones**: Progress logged via sprint highlights & project completions, not daily standups

### Strategic Learning Phases

Instead of tracking 365 individual days, I'm organizing the year into strategic learning phases:

| Phase | Primary Focus                  | Timeline | Key Learning & Projects                                                                                                                                                                               |
| ----- | ------------------------------ | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | Generative AI                  | Jan–Apr  | Completed GenAI Bootcamp · Built multi-agent chatbots, RAG demos, ASR/TTS experiments                                                                                                                 |
| 2     | MCP & Multi-Agent Systems      | May–Jul  | AWS AI Practitioner cert · Networking Bootcamp (multi-VPC design) · Agentic Comic Generator (Hugging Face Hackathon) · LLM Zoomcamp · 100DaysOfCloud Discord Bot · Discord MCP Server · Anthropic MCP |
| 3     | MCP Tooling & Cloud            | Aug–Oct  | Albumentations MCP Server (Kiro Hackathon) · Discord MCP Server · Albumentations MCP VLM feature (Nano Banana Hackathon) · AWS SAA (BeSA) prep · Korean B2 (KSI) · MLOps Zoomcamp · LLM Zoomcamp      |
| 4     | Cloud Practice & Consolidation | Nov–Dec  | 100 Days of Cloud (AWS SkillBuilder + projects) · Kiroween Hackathon (skeleton structure track) · EdgeMind paper finalization · Backlog cleanup (closing open repos)                                  |

> Note: Some tracks (e.g. certifications, Zoomcamps, MCP tools) span multiple phases. Phases are for showcasing emphasis.

---

### 🧱 Projects in Progress

- **100 Days of Cloud (Nov–Dec 2025)**  
  Daily AWS practice log exploring networking, IAM, containers, and GenAI on the cloud.  
  Goal: strengthen AWS fundamentals while applying AI services in real workflows.  
  → [Project Repo](https://github.com/Ramsi-K/100-days-of-cloud-2025)

- **Kiroween Hackathon — Skeleton Structure Track**  
  Building a lightweight MCP-compliant note reader inspired by GoodReader/Notion.  
  Focus: PDF parsing, highlight detection, and automated note syncing to Notion.  
  → [Project Repo](https://github.com/Ramsi-K/kiroween-skeleton) _(placeholder)_

- **LangGraph Mini Project (Planned)**  
  Short RAG-based build to showcase agent orchestration with LangChain + LangGraph.  
  Goal: add one polished, industry-relevant LLM project for job readiness.  
  _(Targeting December as a compact build if bandwidth allows.)_

## 🏆 Completed Projects & Outcomes

### **EdgeMind — AWS Agents Hackathon (Oct 2025)**

5G–6G edge orchestration framework integrating multi-agent swarms with Strands Agents and MEC for sub-100 ms decisioning.

- Built during the AWS Agents Hackathon; now evolving into a research-backed framework for agentic orchestration at the network edge.
- Implements structured agent memory, ReAct-style critique loops, and JSON-based orchestration
- Serves as foundation for an ongoing paper on 6G Edge Intelligence

→ [Project Repo](https://github.com/Ramsi-K/EdgeMind) · [Live Demo](https://ramsik-edgemind.streamlit.app/)

### **BeSA Bootcamp — Migration & Modernization on AWS (Sep–Oct 2025)**

Focused on large-scale migration patterns and modernization strategies across hybrid environments.  
Completed full curriculum including migration waves, VMware Cloud on AWS, and modernization architectures.  
→ [Project Repo](https://github.com/Ramsi-K/100-days-of-cloud-2025) (AWS practice logs)

### **Discord MCP (Proof of Concept)**

A modular, MCP-compliant Discord automation server that bridges AI assistants (Claude, etc.) with Discord for agent-tool orchestration, role-based automation, and workflow management. Explored context persistence, structured prompts, and analytics integration.

Currently in beta testing, consolidating from 26 tools to 9 production-ready modules.

- Implements atomic + workflow-based tools (`discord_send`, `discord_discovery`, `discord_campaign`, etc.)
- Designed for AI assistants to manage communities, run campaigns, and automate Discord workflows
- Features structured SQLite memory, natural-language intent parsing, and Jinja2 templated messaging
- Next phase: optimizing API exposure and formalizing pipeline tests for production readiness
- Deployed successfully across test servers; preparing public beta release

→ [Project Repo](https://github.com/Ramsi-K/discord-mcp)

### Albumentations MCP (Kiro Hackathon, Jul - Sept 2025, Nano Banana Hackathon Sept 2025)

MCP-compliant image augmentation tool using [Albumentations](https://albumentations.ai/).  
Built to enable **safe, auditable augmentation pipelines** driven by natural language prompts.  
Integrated with Nano Banana (Gemini 2.5 VLM) for hybrid image-to-image workflows.

- Natural language → structured transforms (`"add blur and rotate 15 degrees"` → GaussianBlur + Rotate)
- Full MCP protocol support with tools (`augment_image`, `validate_prompt`, `list_available_transforms`, etc.)
- Preset pipelines for segmentation, portrait, and lowlight augmentation
- Deterministic seeding and structured session logging for reproducibility
- VLM integration: Nano Banana/Gemini for vision-language guided edits (`vlm_edit_image`, `vlm_suggest_recipe`)
- Configurable via Claude Desktop, Kiro IDE, and MCP JSON setup
- Robust error handling, logging, and reproducibility hooks
- Documentation: [Architecture Overview](https://github.com/Ramsi-K/albumentations-mcp/blob/main/docs/architecture.md) · [VLM Guide](https://github.com/Ramsi-K/albumentations-mcp/blob/main/docs/vlm_nano_banana.md)

**Tech stack:** Python, Albumentations, MCP, Gemini/Nano Banana, uvx, Kiro IDE

→ [Project Repo](https://github.com/Ramsi-K/albumentations-mcp)

### Hugging Face Hackathon (Jun 2025)

- **Agentic Comic Generator (Hackathon Project)**  
  Hugging Face / LlamaIndex Hackathon submission. A multi-agent comic generation system powered by GPT-4o, SDXL, and LlamaIndex.

  - Dual-agent setup: `Agent Brown` (reasoning + critique) and `Agent Bayko` (image generation via Modal)
  - Custom LlamaIndex event system with persistent memory and structured state logging
  - Modal serverless endpoints for SDXL generation
  - Gradio UI with real-time agent feedback
  - Tech stack: GPT-4o, Mistral Codestral, Hugging Face Diffusers, Modal, Gradio
  - [View Certificate](/certs/other/Certificate-AgentsMCP-Hackathon-1753207993545_8171.png)

  → [Project Repo](https://github.com/Ramsi-K/agentic-comic-generator)

### GenAI Bootcamp (Feb–Apr 2025)

- ✅ **Completed 100% of all project submissions**
- 🔴 **Awarded RED SQUAD recognition** - highest grade awarded
- 📜 [View Certificate](certs/genai-bootcamp/certificate.pdf)
- 🧠 Focus Areas: TOGAF, ASR, TTS, AI assisted Language Learning, Agents, RAG, MUD games, handwriting recognition, multi-agent chatbots
- 💥 Challenges faced:
  - Struggled with frontend/backend integration
  - Major friction with deployment (Docker, Spaces, Firewalls)
  - Learned the importance of understanding cloud tools earlier in project cycles

### **LLM Zoomcamp (DataTalksClub)** _(Partial — Jul–Oct 2025)_

Completed core modules on embeddings, vector databases, and evaluation. Capstone paused due to concurrent hackathons — planned revisit for early 2026.
→ [Course Link](https://github.com/DataTalksClub/llm-zoomcamp)

### AWS Learning Highlights

- 🏅 [AWS Certified AI Practitioner](https://www.credly.com/badges/1f290b70-e366-4756-a959-413c8c3b4398/public_url)
- 🎓 [AWS Cloud Quest: Cloud Practitioner](https://www.credly.com/badges/7de75131-01cf-4d37-851b-cb63f6f39dae/public_url)
- 🏅 [AWS Certified Cloud Practitioner](https://www.credly.com/badges/684fdd1c-105a-4ee4-a472-f15381285ecd/public_url)
- 🤖 [AWS Educate Intro to Generative AI](https://www.credly.com/badges/17ad2294-e69a-4465-9d58-226109158cce/public_url)
- 🗣️ [AWS Skill Builder: Amazon Lex Getting Started](certs/aws/17999_5_861541_1746163529_AWSSkillBuilderCourseCompletionCertificate.pdf)
- 🏅 [BeSA Bootcamp (AWS Migration & Modernization)](./certs/besa-bootcamp/certificate.png)

## 🧪 Certifications Gallery

### LeetCode Monthly Challenge Badges

| Jan                             | Feb                             | Mar                             | Apr                             | May                             | Jun                             |
| ------------------------------- | ------------------------------- | ------------------------------- | ------------------------------- | ------------------------------- | ------------------------------- |
| ![](certs/leetcode/2025-01.png) | ![](certs/leetcode/2025-02.png) | ![](certs/leetcode/2025-03.png) | ![](certs/leetcode/2025-04.png) | ![](certs/leetcode/2025-05.png) | ![](certs/leetcode/2025-06.png) |
| Jul                             | Aug                             | Sep                             | Oct                             | Nov                             | Dec                             |
| ![](certs/leetcode/2025-07.png) | ![](certs/leetcode/2025-08.png) | **n/a**                         | ![](certs/leetcode/2025-10.png) |                                 |                                 |

---

### AWS Certifications

| AI Practitioner                                  | Cloud Practitioner                                  | Cloud Quest                                           | Intro to GenAI                                               |
| ------------------------------------------------ | --------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------ |
| ![](certs/aws/aws-certified-ai-practitioner.png) | ![](certs/aws/aws-certified-cloud-practitioner.png) | ![](certs/aws/aws-cloud-quest-cloud-practitioner.png) | ![](certs/aws/aws-educate-introduction-to-generative-ai.png) |

---

### Other Certifications

- [Introduction to Model Context Protocol](/certs/other/Introduction%20to%20Model%20Context%20Protocol.pdf)
- [Model Context Protocol: Advanced Topics](/certs/other/Model%20Context%20Protocol%20Advanced%20Topics.pdf)
- [MCP: Build Rich-Context AI Apps with Anthropic](https://learn.deeplearning.ai/accomplishments/b3ea9e3f-114a-4a5d-a00a-071ac3f3c30a?usp=sharing)
- [Practical Multi AI Agents and Advanced Use Cases with crewAI](https://learn.deeplearning.ai/accomplishments/5686ef40-8d2f-41be-9f46-08d60f0b1550?usp=sharing)
- [Korean Introductory Course KSI](/certs/other/KSI%20Introductory.pdf)
- [MLOps Zoomcamp](certs/other/DataTalks%20MLOps%20Zoomcamp.pdf)

---

## 📘 Research Papers

- “EdgeMind: Multi-Agent Orchestration in the Transition from 5G to 6G” → in progress
- “Turn Detection in AI Language Learning” → [Dissertation Link](https://www.academia.edu/128366473/Turn_Detection_in_AI_Powered_Language_Learning_Cultural_Neurodivergent_and_Ethical_Implications)
- “Beyond Human Mimicry: Rethinking AI Identity” → in progress
- Additional breakdowns from GenAI bootcamp to be published on [arXiv](https://arxiv.org/) or [Academia.edu](https://independentscholar.academia.edu/RamsiKalia)

### 🧪 Exploratory Topics

- **CFD Memory**  
  Investigating fluid-inspired memory systems where contextual relevance emerges from dynamic flow patterns rather than static vector weights.  
  _Focus:_ memory decay, attention turbulence, and mesh-based semantic diffusion.

- **Korea as an AI Testbed**  
  Exploring South Korea’s unique role as a contained ATS-friendly deployment zone for multilingual AI tooling.  
  _Emphasis:_ linguistic modeling, policy alignment, and interface testing across hyper-digital infrastructure.

---

## 📁 Repository Structure

- `leetcode/` → [LeetCode Daily Solutions (Submodule)](https://github.com/yourusername/leetcode-solutions)
- `certs/`
  - `leetcode/` → Monthly certificate images
  - `aws/` →
- `bootcamps/`
  - `genai/` → [GenAI Bootcamp Repo](bootcamps/genai)
  - `networking/` → [Networking Bootcamp Repo](bootcamps/networking)
- `courses/`
  - `*` → Optional self-paced courses
  <!-- - `papers/` – Research breakdowns, dissertations, longform writing -->

---

## 🔗 Useful Links

- [GenAI Bootcamp Journal](https://github.com/Ramsi-K/free-genai-bootcamp-2025/blob/main/journal.md)
- [LinkedIn](https://www.linkedin.com/in/ramsikalia/)
- [Academia.edu](https://independentscholar.academia.edu/RamsiKalia)

---

> ## Connect & Collaborate
>
> I believe in learning in public and welcome collaboration. If you're interested in any of the projects or want to pair program on anything, you can reach out to me via [LinkedIn](https://www.linkedin.com/in/ramsikalia/).
