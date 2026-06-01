# 🪐 SolPlus Agent — Enterprise Autonomous Intelligence Platform

An advanced Web3 infrastructure blueprint combining autonomous agent orchestration, machine learning data engines, and secure transaction clearing mechanisms. Built natively for the Solana Network utilizing the OOBE Protocol framework and Ace Data Cloud inference pipelines.

---

## 🏛️ System Architecture Topology

The application is structured linearly across four distinct operational layer paradigms:

1. **Orchestration Layer (`src/lib/agent/Engine`)**
   Queries blockchain registry systems to discover specialized tools, handles data aggregation streams via the Synapse protocol, evaluates execution conditions, and triggers actions.

2. **Intelligence Layer (`src/lib/ai/AceDataEngine`)**
   Processes complex, raw pool performance statistics using parallel API queries to extract definitive market sentiment vector weights and categorization taxonomies.

3. **Data Persistency Layer (`prisma/schema.prisma`)**
   An object-relational schema built over a robust PostgreSQL cluster. It logs real-time workflow step metrics, user agent states, structural telemetry data, and settlement information.

4. **Interface Matrix Layer (`src/app/` & `src/components/ui/`)**
   A high-performance Next.js application wrapper enhanced with Tailwind CSS utility classes, real-time HTML5 Canvas network nodes, and Framer Motion layouts.

---

## ⚙️ Environmental Configurations Matrix

Create a local, non-tracked environment variables storage configuration file named `.env` in the root folder. It must contain the following parameters to connect successfully to external clusters:

```env
# System Server Networks
PORT=3000
NODE_ENV=production

# Database Infrastructure Layout
DATABASE_URL="postgresql://solplus_admin:SecretProductionPasswordVaultXYZ112@solplus-db:5432/solplus_intelligence_db?schema=public"

# On-Chain Protocols & Web3 Gateways
SOLANA_RPC_URL="[https://api.mainnet-beta.solana.com](https://api.mainnet-beta.solana.com)"
SYNAPSE_RPC_URL="[https://synapse.mainnet.oobe.protocol](https://synapse.mainnet.oobe.protocol)"

# Machine Learning & AI Core Model Keys
ACE_DATA_CLOUD_API_KEY="ace_live_sec_prod_alpha_matrix_key"

# Instant Alert Distribution Webhooks
TELEGRAM_BOT_TOKEN="0000000000:AA-YourLiveProductionTelegramBotTokenKeyHere"
TELEGRAM_CHAT_ID="-100xxxxxxxxx"
# Navigate to project root folder
cd solplus-agent

# Create environment configuration file
touch .env
nano .env # Paste your environment variables matrix here

# Force fresh construction of system container layers
docker-compose up -d --build

# Synchronize database tables to look exactly like your prisma schema
npx prisma migrate deploy

# Synchronize database tables to look exactly like your prisma schema
npx prisma migrate deploy

  docker compose logs -f solplus-app

  docker compose exec solplus-db pg_isready -U solplus_admin

  npx prisma db push --force-reset
