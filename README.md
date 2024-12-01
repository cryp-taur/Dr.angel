# Dr.angel 🏥

<div align="center">
  <img src="./docs/static/img/angel_banner.jpg" alt="Angel Banner" width="100%" />
</div>

  
</div>

# Angel Function Overview

Angel is a repair and optimization-based Agent AI assistant built on the Eliza open-source model, designed to provide optimization solutions for decentralized AI models. It relies on Claude's powerful code review and repair capabilities, along with a self-developed open-source web crawler technology, to assist any Agent in optimizing code and providing a knowledge base for enhancement.

---

## Features

Angel offers a range of powerful features to help users quickly integrate across multiple platforms, flexibly manage Agents, and automatically optimize command sets. With strong AI models and custom support, users can easily tailor and expand their own smart assistants.

- 🔗 **Multi-Platform Connection**  
  Supports platforms like Discord, Twitter, and Telegram, helping users easily connect and manage AI assistants across different channels.

- 🧠 **Multimodal Agent Support**  
  Handles different types of tasks and interactions flexibly, supporting task execution in various modalities to assist in more complex business processes.

- 📂 **Document Interaction**  
  Easily import documents, and Angel can interact with them efficiently to help users understand and use relevant materials.

- 💾 **Smart Storage**  
  Provides a searchable memory and document storage system, ensuring information is always available, aiding users in quickly accessing and managing historical data.

- 🚀 **Highly Scalable**  
  Highly customizable, supporting client and behavior extensions, allowing users to expand functionality according to their needs and meet personalized requirements.

- 🌍 **Multi-Model Compatibility**  
  Supports a variety of models such as Llama, OpenAI, Grok, and Anthropic, allowing users to switch models flexibly to achieve optimal results.

- 🛠 **Easy to Use**  
  Angel features a clean and user-friendly design, enabling users to quickly get started and easily customize and extend their AI assistant's features.

---

## What Can You Do with Angel?

Angel has flexible functionality, making it suitable for various scenarios, helping users improve work efficiency, automate management, and optimize task execution.

- 💬 **Open Source Project Query**  
  Quickly search for information on current open-source Agent projects, helping you stay up to date with project dynamics and the latest technology news.

- 🕵️ **Autonomous Task Execution**  
  Create and manage autonomous Agents based on your needs, executing various tasks to improve work efficiency.

- 📚 **Self-Improving Knowledge Base**  
  Recognize Agent intents and instructions, automatically improving the knowledge base to keep knowledge up-to-date and accurate.

---

## Highlight Features

Angel's highlight features include its ability to deeply repair and optimize Agents while intelligently improving the knowledge base, ensuring continuous evolution of each Agent.

- 🔧 **Agent Health Check and Repair**  
  Using Claude's powerful code review feature, Angel automatically repairs Agent instruction errors and optimizes code structure. In this way, Angel helps any Agent improve efficiency and accuracy.

- 📖 **Knowledge Base Feeding**  
  Based on current Agent instruction sets, Angel generates optimized command sets and uses self-developed open-source web crawlers to gather information, constructing an enhanced knowledge base document that helps Agents expand their knowledge and improve execution.

---

## Getting Started

Before using Angel, you need to perform some basic configurations. Follow the steps below to easily start and experience the powerful Agent features.

### Prerequisites

1. **Node.js 23+**  
2. **pnpm**: Install dependencies using pnpm.
3. **Environment Configuration**: Edit the `.env` file by copying `.env.example` to `.env` and filling in the appropriate values.
4. **Character Files**: Check `src/core/defaultCharacter.ts` and modify the character configuration.  
   You can also use the following command to load characters and run multiple bots simultaneously:

   ```bash
   node --loader ts-node/esm src/index.ts --characters="path/to/your/character.json"
