# Claude Skill: Perplexity Prompting

A comprehensive Claude Skill that teaches effective use of Perplexity MCP tools for internet-native research and discovery. This skill transforms how Claude uses Perplexity by teaching 8 essential prompting strategies and best practices for getting the most accurate, verifiable, and useful results.

## What This Skill Teaches

This skill trains Claude to:

- **Optimize queries before execution** - Engage in exploratory conversations to understand user needs and craft better queries
- **Apply 8 key prompting strategies** - Including progressive deepening, exact search parameters, multiple perspectives, and avoiding hallucinations
- **Choose the right tool** - Select between `perplexity_ask`, `perplexity_research`, `perplexity_reason`, and `perplexity_search` based on the task
- **Understand Perplexity's unique nature** - Recognize it as an internet-first research tool (not just a middle ground between Google and ChatGPT)
- **Reduce hallucinations** - Use specific techniques to ensure verifiable, sourced, and accurate information

## Why This Matters

Perplexity is fundamentally different from ChatGPT:

- **ChatGPT**: Looks inside its training data first (inward-focused)
- **Perplexity**: Searches the entire internet first (outward-focused)
- **Method**: Uses Retrieval Augmented Generation (RAG) - searches → finds sources → extracts info → crafts answers with citations

This skill helps Claude leverage these differences effectively, producing better research results with verifiable sources.

## Prerequisites

You must install the [Perplexity MCP server](https://docs.perplexity.ai/guides/mcp-server) before using this skill.

## Installation

### Option 1: Claude Desktop Capabilities (Recommended)

1. Go to the [Releases page](../../releases) and download the latest `perplexity-prompting-skill-*.zip` file
2. In Claude Desktop, open **Settings** → **Capabilities**
3. Upload the zip file to add the skill
4. The skill will be available immediately

### Option 2: Manual Installation

1. Download the latest release zip or clone this repository
2. Extract or copy the `.claude/skills/perplexity_prompting/` directory to:
   - **For a specific project:** Your project's `.claude/skills/` directory (for Claude Code)
   - **For global use:** Your `~/.claude/skills/` directory (works with both Claude Desktop and Claude Code)
3. Restart Claude if needed to load the new skill

## Usage

Once installed, Claude will automatically use this skill when:

- You explicitly mention Perplexity
- You request current web information, breaking news, or competitive intelligence
- You need academic research with recent developments
- You ask for verifiable sourced answers with citations
- You're working with the Perplexity MCP tools

### Example Interaction

**Instead of this:**
```
User: "Find me recent news on AI"
Claude: [executes generic query, gets poor results]
```

**The skill enables this:**
```
User: "Use perplexity to find me recent news on AI"
Claude: "I'd love to help you research AI developments. Let's start with what
matters most to you - what specific area of AI are you interested in?"
[Exploratory conversation continues...]
Claude: "Based on our conversation, here's my recommended query: 'Find diverse,
well-grounded novel AI updates since October 2025 focused on developer tools
and frameworks, from at least 3 different industry sources.'
This uses Strategy #1 (context), Strategy #3 (exact dates), and Strategy #4
(multiple perspectives). Does this capture what you're looking for?"
```

## The 8 Essential Strategies

The skill teaches 8 key Perplexity prompting techniques:

1. **A Little Context Goes a Long Way** - Adding 2-3 words of context can dramatically improve results
2. **NEVER Use Few-Shot Prompting** - Don't give examples (unlike ChatGPT)
3. **Use Exact Search Parameters** - Specify dates, source types, and constraints precisely
4. **Demand Multiple Perspectives** - Force triangulation instead of single-source answers
5. **Progressive Deepening** - Start broader, then drill down through conversation
6. **Specify Output Constraints** - Reduce hallucinations by requiring specific citations
7. **Strategic Focus Mode Usage** - Switch modes to reset thinking while keeping context
8. **Create Custom Workflows** - Structure recurring research patterns consistently

## Best Use Cases

Perplexity excels at:

- Competitive intelligence and market research
- Stock and financial analysis
- Breaking news and current events
- Academic research with recent developments
- Discovering unexpected connections
- Any situation needing internet-first, up-to-date information

## Project Structure

```
.
├── README.md                          # This file
├── CLAUDE.md                          # Project instructions for Claude Code
├── .claude/
│   └── skills/
│       └── perplexity_prompting/
│           └── SKILL.md               # The actual skill definition
└── sources/                           # Reference materials
    ├── nate-b-jones-master-perplexity-prompting.md
    └── installing-perplexity-mcp-server.md
```

## Development

This is a documentation-only project with no build system or code to run. Development consists of:

1. Researching Perplexity usage patterns from source materials
2. Writing and refining the SKILL.md file
3. Testing with real Claude interactions
4. Maintaining reference documentation

## Contributing

Contributions are welcome! Areas for improvement:

- Additional real-world examples
- New prompting strategies or techniques
- Better tool selection guidance
- Updated best practices as Perplexity evolves

## Credits

This skill is based on the excellent article ["Master Perplexity Prompting"](sources/nate-b-jones-master-perplexity-prompting.md) by Nate B. Jones, which provides deep insights into Perplexity's unique characteristics and effective usage patterns.

## License

MIT License - See LICENSE file for details
