# Gptscript with Supabase API and CLI

Welcome to the Gptscript project! This guide will help you understand how to use Gptscript to interact with Supabase APIs and CLI.

## Overview

Gptscript is a friendly assistant designed to help you with DevOps-related tasks using CLI programs. In this project, Gptscript is configured to assist with Supabase API and CLI operations.

## Prerequisites

Before you begin, ensure you have the following:

- [Supabase API key](https://supabase.com/docs/reference/api/introduction)
- [Supabase CLI installed](https://supabase.com/docs/guides/cli/getting-started)

## Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/gptscript-ai/supabase-agent.git
   cd supabase-agent
   ```

2. **Set Up Environment Variables:**
   You need to set up your Supabase API key as an environment variable.
   ```bash
   export GPTSCRIPT_API_SUPABASE_COM_BEARER_AUTH="your-supabase-api-key"
   ```

## Using Gptscript with Supabase API

Gptscript can help you navigate and use the Supabase API. The `.gpt` files define the capabilities and context for Clio.

### Available Commands

- **General API Helper:**

  - File: `tool.gpt`
  - Description: Helps with all Supabase API operations.
  - Tools: All tools from `openapi.yaml`.

- **Read Operations:**

  - File: `tool-api-read.gpt`
  - Description: Helps with read operations in Supabase API.
  - Tools: `v1-get*`, `v1-list*` from `openapi.yaml`.

- **Write Operations:**
  - File: `tool-api-write.gpt`
  - Description: Helps with write operations in Supabase API.
  - Tools: `v1-create*`, `v1-update*`, `v1-delete*` from `openapi.yaml`.

### Example Usage

To use Gptscript for Supabase API operations, you can direct a message to the specific agent. For example:

```bash
gptscript ./tool-api-all.gpt
```

## Using Gptscript with Supabase CLI

Gptscript can also assist with Supabase CLI commands. The `supabase-cli.gpt` file defines the context for CLI operations.

### Available Commands

- **CLI Helper:**
  - File: `tool-cli.gpt`
  - Description: Helps with Supabase CLI operations.
  - Context: `cli-helper`

### Example Usage

To use Gptscript for Supabase CLI operations, you can direct a message to the specific agent. For example:

```bash
Gptscript ./tool-cli.gpt
```

## Conclusion

Gptscript is here to make your interaction with Supabase APIs and CLI easier. If you have any questions or need further assistance, feel free to ask Clio for help.
