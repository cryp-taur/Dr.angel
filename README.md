# TANis_STAN☠️

<div align="center">
  <img src="./docs/static/img/angel_banner.jpg" alt="Angel Banner" width="100%" />
</div>

  
</div>

# TANIS Function Overview
TANIS is an AI from hell💀TANIS is a repair and optimization-based Agent AI assistant built on the Eliza open-source model, designed to provide optimization solutions for decentralized AI models. It relies on Claude's powerful code review and repair capabilities, along with a self-developed open-source web crawler technology, to assist any Agent in optimizing code and providing a knowledge base for enhancement.

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
pnpm i
pnpm start

Customizing Angel
Angel supports flexible custom operations. You can configure behaviors, select different large models, and optimize your Agent experience according to your needs.

Adding Custom Behaviors
To avoid conflicts with the core directory's Git, it's recommended to add custom operations to the custom_actions directory and configure them in the angelConfig.yaml file. You can refer to the example in angelConfig.example.yaml.

Configuring Different Large Models
Llama Configuration
Set the XAI_MODEL environment variable to meta-llama/Meta-Llama-3.1-70B-Instruct-Turbo or meta-llama/Meta-Llama-3.1-405B-Instruct to run the Llama model.

OpenAI Configuration
Set the XAI_MODEL environment variable to gpt-4o-mini or gpt-4o to run the OpenAI model.

Other Dependencies
If you encounter errors when starting, try installing sharp:
pnpm install --include=optional sharp
Environment Configuration
Configure the following environment variables in the .env file to connect various platforms:
# Required environment variables
DISCORD_APPLICATION_ID=
DISCORD_API_TOKEN= # Bot token
OPENAI_API_KEY=sk-* # OpenAI API key, starting with sk-
ELEVENLABS_XI_API_KEY= # Elevenlabs API key

# ELEVENLABS Settings
ELEVENLABS_MODEL_ID=eleven_multilingual_v2
ELEVENLABS_VOICE_ID=21m00Tcm4TlvDq8ikWAM
ELEVENLABS_VOICE_STABILITY=0.5
ELEVENLABS_VOICE_SIMILARITY_BOOST=0.9
ELEVENLABS_VOICE_STYLE=0.66
ELEVENLABS_VOICE_USE_SPEAKER_BOOST=false
ELEVENLABS_OPTIMIZE_STREAMING_LATENCY=4
ELEVENLABS_OUTPUT_FORMAT=pcm_16000

TWITTER_DRY_RUN=false
TWITTER_USERNAME= # Twitter account
TWITTER_PASSWORD= # Twitter password
TWITTER_EMAIL= # Twitter email
TWITTER_COOKIES= # Twitter Cookies

X_SERVER_URL=
XAI_API_KEY=
XAI_MODEL=


# Other API Configurations
ANTHROPIC_API_KEY=

# EVM Configuration
EVM_PRIVATE_KEY=EXAMPLE_WALLET_PRIVATE_KEY

# Solana Configuration
SOLANA_PRIVATE_KEY=EXAMPLE_WALLET_PRIVATE_KEY
SOLANA_PUBLIC_KEY=EXAMPLE_WALLET_PUBLIC_KEY

# Local Wallet Configuration (deprecated)
WALLET_PRIVATE_KEY=EXAMPLE_WALLET_PRIVATE_KEY
WALLET_PUBLIC_KEY=EXAMPLE_WALLET_PUBLIC_KEY

BIRDEYE_API_KEY=

SOL_ADDRESS=So11111111111111111111111111111111111111112
SLIPPAGE=1
RPC_URL=https://api.mainnet-beta.solana.com
HELIUS_API_KEY=


## Telegram Configuration
TELEGRAM_BOT_TOKEN=

TOGETHER_API_KEY=
Local Configuration
CUDA Configuration
If you have a high-performance NVIDIA graphics card, you can accelerate local operations via CUDA:
pnpm install
npx --no node-llama-cpp source download --gpu cuda
Make sure you have installed the complete CUDA toolkit, including cuDNN and cuBLAS.

Running Locally
Set the XAI_MODEL to one of the aforementioned Llama models. You can leave X_SERVER_URL and XAI_API_KEY empty, and the model will be downloaded from Hugging Face and run locally.

Client Setup
For setting up a Discord bot, it's recommended to refer to the official Discord documentation.

Development & Testing
Testing Commands
Common test commands:
pnpm test           # Run tests once
pnpm test:watch    # Run tests in watch mode
Database-specific test commands:
pnpm test:sqlite   # Test with SQLite
pnpm test:sqljs    # Test with SQL.js
ests are written with Jest and are located in the src/*/.test.ts files. The test environment is configured as follows:

Loads environment variables from .env.test
Sets a 2-minute timeout for long-running tests
Supports ESM modules
Runs tests in sequence (--runInBand)
To add new tests, add a .test.ts file next to the relevant code.
