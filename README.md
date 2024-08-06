# Clio with Supabase API and CLI

Welcome to the Clio project! This guide will help you understand how to use Clio to interact with Supabase APIs and CLI.

## Overview

Clio is a friendly assistant designed to help you with DevOps-related tasks using CLI programs. In this project, Clio is configured to assist with Supabase API and CLI operations.

## Prerequisites

Before you begin, ensure you have the following:

- Supabase API key
- Supabase CLI installed

## Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/gptscript-ai/supabase-agent.git
   cd supabase-agent
   ```

2. **Set Up Environment Variables:**
   You need to set up your [Supabase API key](https://supabase.com/docs/reference/api/introduction) as an environment variable.
   ```bash
   export GPTSCRIPT_API_SUPABASE_COM_BEARER_AUTH="your-supabase-api-key"
   ```

## Using Clio with Supabase API

Clio can help you navigate and use the Supabase API. The `.gpt` files define the capabilities and context for Clio.

### Available Commands

- **General API Helper:**

  - File: `supabase-api-all.gpt`
  - Description: Helps with all Supabase API operations.
  - Tools: All tools from `openapi.yaml`.

- **Read Operations:**

  - File: `supabase-api-read.gpt`
  - Description: Helps with read operations in Supabase API.
  - Tools: `v1-get*`, `v1-list*` from `openapi.yaml`.

- **Write Operations:**
  - File: `supabase-api-write.gpt`
  - Description: Helps with write operations in Supabase API.
  - Tools: `v1-create*`, `v1-update*`, `v1-delete*` from `openapi.yaml`.

### Example Usage

To use Clio for Supabase API operations, you can direct a message to the specific agent. For example:

```bash
clio ./supabase-api-all.gpt
```

## Using Clio with Supabase CLI

Clio can also assist with Supabase CLI commands. The `supabase-cli.gpt` file defines the context for CLI operations.

### Available Commands

- **CLI Helper:**
  - File: `supabase-cli.gpt`
  - Description: Helps with Supabase CLI operations.
  - Context: `cli-helper`

### Example Usage

To use Clio for Supabase CLI operations, you can direct a message to the specific agent. For example:

```bash
clio ./supabase-cli.gpt
```

## Conclusion

Clio is here to make your interaction with Supabase APIs and CLI easier. If you have any questions or need further assistance, feel free to ask Clio for help.
