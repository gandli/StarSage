# StarSage

<p align="center">
  <img src="src/assets/icon.png" height="128" alt="StarSage icon">
</p>

<p align="center">
  <a href="https://github.com/gandli/star-sage-app/actions/workflows/deploy.yml">
    <img src="https://github.com/gandli/star-sage-app/actions/workflows/deploy.yml/badge.svg" alt="Deploy to GitHub Pages">
  </a>
  <img src="https://img.shields.io/badge/react-19-blue" alt="React 19">
  <img src="https://img.shields.io/badge/supabase-2.x-green" alt="Supabase">
</p>

<p align="center">
  <strong>StarSage</strong> is a high-performance, multi-user starred repository management dashboard designed for GitHub enthusiasts. Through extreme rendering performance, intelligent information organization and multi-user collaboration, it brings new life to your GitHub knowledge base.
</p>

![overview](src/assets/overview.png)

## ✨ Core Features

- **🚀 Extreme Performance Engine**:
  - **Native Theme Integration**: CSS variable-driven, zero-flicker dark/light mode
  - **Concurrent Rendering Optimization**: React 19 concurrent mode for tens of thousands of items
  - **Lightning-fast Access**: IndexedDB local caching + Supabase cloud sync

- **👥 Multi-user Collaboration**:
  - **Independent Star Management**: Each user has independent star lists
  - **Shared Translation Pool**: Repository descriptions shared globally
  - **Intelligent Data Isolation**: RLS-based data security isolation

- **🧠 Intelligent Enhancement**:
  - **AI Translation Pipeline**: Auto-translates repository descriptions via a Cloudflare Worker translation service
  - **Smart Search & Filtering**: Fast full-text search across your entire star knowledge base
  - **Insight Charts**: Language and activity analytics powered by Recharts

## 🛠️ Tech Stack

- React 19 + TypeScript + Vite
- Tailwind CSS + shadcn-style components
- Supabase (auth, Postgres, RLS) + IndexedDB (`idb`) for local cache
- Recharts for data visualization
- Vitest for unit testing

## 🚀 Getting Started

### Prerequisites

- [Bun](https://bun.sh/) (or Node.js 20+)
- A Supabase project (URL + anon key)

### Setup

1. Clone and install dependencies:

```bash
git clone https://github.com/gandli/star-sage-app.git
cd star-sage-app
bun install
```

2. Configure environment variables — copy `.env.example` to `.env` and fill in:

```text
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

3. Start the dev server:

```bash
bun run dev
```

4. Build for production:

```bash
bun run build
```

5. Run tests:

```bash
bun run test
```

## 📄 License

All rights reserved.
