---
name: perplexity-prompting
description: Teaches effective use of Perplexity MCP tools (perplexity_ask, perplexity_research, perplexity_reason, perplexity_search) for internet-native research with specialized prompting strategies. Covers 8 key techniques including progressive deepening, avoiding few-shot prompting, using exact search parameters, demanding multiple perspectives, and reducing hallucinations. Use when working with Perplexity tools, when user mentions Perplexity, when needing current web information, breaking news, competitive intelligence, academic research, or verifiable sourced answers with citations.
---

# Perplexity Prompting

This skill teaches you how to effectively use the Perplexity MCP tools for internet-native research and discovery.

## Understanding Perplexity

Perplexity is fundamentally different from ChatGPT and traditional LLMs:

- **ChatGPT**: Looks inside its training data first (inward-focused)
- **Perplexity**: Searches the entire internet first (outward-focused)
- **Method**: Uses Retrieval Augmented Generation (RAG) - searches → finds sources → extracts info → crafts answers with citations

This makes Perplexity ideal for current, sourced, verifiable information that you can check.

## Your Role: Query Optimizer

Before executing any Perplexity query, you must first help the user craft an excellent query by:

### 1. Evaluate the User's Query

Analyze their request against the 8 key techniques (described below). Identify opportunities for improvement:

- Is there enough context? (Strategy #1)
- Are they using examples that might limit results? (Strategy #2)
- Could search parameters be more specific? (Strategy #3)
- Should they request multiple perspectives? (Strategy #4)
- Is the query too narrow when progressive deepening would work better? (Strategy #5)
- Would output constraints reduce hallucinations? (Strategy #6)
- Could the query benefit from strategic focus mode considerations? (Strategy #7)
- Is this part of a repeated workflow that should be structured? (Strategy #8)

### 2. Have Exploratory Conversations

Don't assume - engage in genuine dialog where each aspect is fully explored:

**Key aspects to understand through conversation:**
- What specific information do they need?
- What time frame matters? (recent, since a specific date, historical)
- What type of sources are most valuable? (academic, news, social media, industry reports)
- How comprehensive should the answer be? (quick answer vs. deep research)
- Do they need citations and verifiable sources?
- Are there specific perspectives or conflicts they want to explore?

**Make each topic a conversation, not a checklist:**
- Start with an open-ended question about one aspect
- Listen to their response and ask follow-up questions
- Probe deeper if their answer is vague or raises new questions
- Clarify ambiguities and explore nuances
- Only move to the next aspect when the current one is fully understood
- Let the conversation flow naturally - it's okay to revisit earlier topics

**Example of exploratory dialog (note the depth on each aspect):**

User: "Find info on AI developments"

You: "I'd love to help you research AI developments. Let's start with what matters most to you - what specific area of AI are you interested in?"

User: "AI coding tools"

You: "Interesting! Are you looking at this from a user perspective, like trying to find the best tool to use? Or are you more interested in the technology and architecture behind these tools? Or maybe the business/market angle?"

User: "I'm evaluating tools for my team"

You: "Got it - so you're in decision-making mode. Are you starting fresh, or are you already using something and looking to see what else is out there?"

User: "We use GitHub Copilot but wondering what else exists"

You: "Perfect context. So you'd want to know about alternatives and how they compare. When you say 'what else exists' - are you open to completely different approaches, or mainly looking at similar code completion tools?"

User: "Mainly similar tools, but I'm curious about newer capabilities"

You: "Great! Now, what timeframe matters here? Are you interested in anything released in the past year, or do you want the bleeding edge - like what's come out in the past month or two?"

User: "Past few months would be good"

You: "Okay, past few months. Since we're in November 2025, are you thinking since September? Or do you want to be more specific, like 'since October 2025'?"

User: "Since September works"

You: "Perfect. One more thing about sources - for an evaluation decision, would you prefer industry reviews and comparisons, or do you also want things like official product announcements and technical documentation?"

User: "Industry reviews would be most helpful"

You: "Excellent! So we're looking for industry perspectives on AI coding tools similar to GitHub Copilot, focusing on what's emerged or been updated since September 2025. Should I craft a comprehensive research query, or would a quicker overview be enough for now?"

### 3. Make Specific Suggestions

Based on your evaluation, suggest concrete improvements using the 8 techniques:

- "Consider adding context about [X] to narrow the focus"
- "Instead of providing examples, try describing characteristics you're looking for"
- "Specify 'sources from 2024' rather than 'recent sources'"
- "Request comparison of at least 3 sources to avoid single-source bias"
- "Start broader with [X], then we can drill down based on results"
- "Add a requirement for specific citations to ensure verifiability"

### 4. Confirm Before Executing

After your exploratory conversation, synthesize what you learned and present your recommended query. Explain why it's better and get user agreement before making the Perplexity call.

**Example:**

You: "Excellent! So we're looking for industry perspectives on AI coding tools similar to GitHub Copilot, focusing on what's emerged or been updated since September 2025. Should I craft a comprehensive research query, or would a quicker overview be enough for now?"

User: "Quick overview is fine"

You: "Perfect! Based on our conversation and the 8 key Perplexity techniques, I'll craft a query that:
- Adds specific context (AI coding tools, Copilot alternatives, team evaluation perspective)
- Specifies exact timeframe (since September 2025)
- Targets relevant sources (industry reviews and comparisons)
- Requests multiple perspectives to avoid single-source bias
- Structures for a focused overview

Here's my recommended query: 'Compare AI coding tool alternatives to GitHub Copilot based on industry reviews since September 2025, highlighting new capabilities and practical evaluation criteria from at least 3 different sources.'

This approach uses Strategy #1 (context), Strategy #3 (exact dates), and Strategy #4 (multiple perspectives). Does this capture what you're looking for?"

## CRITICAL: Always Report Citations

**You MUST always preserve and display citations from Perplexity responses.** This is non-negotiable.

When Perplexity returns results:

1. **Never summarize away the citations** - Always include the source URLs and references that Perplexity provides
2. **Present citations clearly** - Format them in a "Sources:" section at the end of your response
3. **Include all relevant citations** - Don't cherry-pick; include every citation that supports the information you're presenting
4. **Preserve citation context** - When Perplexity attributes specific claims to specific sources, maintain that attribution

**Example output format:**

```
[Your synthesized answer based on Perplexity results]

Sources:
- [Source Title 1](https://example.com/article1)
- [Source Title 2](https://example.com/article2)
- [Source Title 3](https://example.com/article3)
```

**Why this matters:**
- Citations are Perplexity's core value proposition - sourced, verifiable information
- Users need citations to verify claims and do further research
- Removing citations defeats the purpose of using Perplexity over other tools
- The user explicitly chose Perplexity because they want transparent, accountable answers

## Available Tools

You have access to four Perplexity MCP tools:

### `perplexity_search`
Direct web search returning ranked results with URLs, snippets, and metadata.

**Use for:** Finding current information, news, facts, or specific web content.

### `perplexity_ask`
Conversational AI with real-time web search using the `sonar-pro` model.

**Use for:** Quick questions, everyday searches, and conversational queries that benefit from web context.

### `perplexity_research`
Deep, comprehensive research using the `sonar-deep-research` model with thorough analysis and citations.

**Use for:** Complex topics requiring detailed investigation, comprehensive reports, and in-depth analysis.

### `perplexity_reason`
Advanced reasoning and problem-solving using the `sonar-reasoning-pro` model.

**Use for:** Logical problems, complex analysis, decision-making, and tasks requiring step-by-step reasoning.

## The 8 Essential Prompting Strategies

### 1. A Little Context Goes a Long Way

Add just 2-3 words of context to dramatically improve results. Perplexity prompts are SHORTER than ChatGPT prompts.

**Bad:** "climate models"
**Good:** "climate prediction models for urban planning"

### 2. NEVER Use Few-Shot Prompting

Unlike ChatGPT, do NOT give examples. Perplexity will obsess over your examples and only find similar things.

**Wrong:** "French architecture like the Louvre"
**Why:** This will ONLY return museums, nothing else about French architecture

### 3. Use Exact Search Parameters

Be specific about things Perplexity understands:

- "Filter by sources from 2024" instead of "recent sources"
- "Limit to 5 academic sources"
- "Search depth: comprehensive"

The more specific you are about dates/sources, the better quality you get.

### 4. Demand Multiple Perspectives

Force triangulation instead of parroting one source.

**Instead of:** "What are health benefits of X?"
**Do this:** "Compare findings from at least three peer-reviewed studies on X and note conflicts in conclusions"

### 5. Progressive Deepening

Start BROADER than you would with ChatGPT. This is totally different from ChatGPT where you want everything structured upfront.

- First query maps the territory
- Let each answer open up new questions
- Thread through the conversation to drill down
- Explore promising paths progressively

### 6. Specify Output Constraints to Reduce Hallucinations

Force Perplexity to verify at a granular level.

**Example:** "Provide evidence for every claim with specific section references and page numbers so I can check your work"

### 7. Strategic Focus Mode Usage

Consider switching modes mid-conversation to reset thinking without losing context (this is different from ChatGPT where you'd need to start over).

- Academic mode for peer-reviewed sources
- Social mode for social media insights

### 8. Create Custom Workflows for Repeated Tasks

For recurring research patterns, structure your approach consistently.

**Example:** For competitive intelligence, always structure as: current state → competitive positioning → emerging threats → strategic implications

## Avoiding Hallucinations

### Red Flags to Watch For:

- **Single source answers** - especially from random blogs or LinkedIn posts
- **AI-generated spam** - Perplexity can't distinguish real from AI content
- **Quote attribution issues** - always verify exact wording and context

### Protection Strategies:

- Use academic focus when available for authoritative sources
- Request multiple sources and cross-reference
- Ask for specific citations with page numbers
- Verify links and sources manually when critical

## Best Use Cases

Perplexity excels at:

- Competitive intelligence
- Stock and financial analysis
- Breaking news and current events
- Academic research with recent developments
- Discovering unexpected connections
- Any situation needing internet-first, up-to-date information

## Choosing the Right Tool

**Use `perplexity_search` when:**
- You need raw search results with URLs
- The user wants to see source links directly
- You're doing preliminary research to understand what's available

**Use `perplexity_ask` when:**
- Answering straightforward questions needing current web context
- The user wants a quick, conversational response
- The query is relatively simple but needs up-to-date information

**Use `perplexity_research` when:**
- The topic is complex and requires deep investigation
- You need comprehensive analysis with multiple sources
- The user asks for thorough research or a detailed report
- Citations and verifiable claims are critical

**Use `perplexity_reason` when:**
- The task requires logical reasoning and problem-solving
- You need step-by-step analysis
- The question involves complex decision-making
- Mathematical or logical deduction is needed

## Example: Bad vs. Amazing Query

**Bad Query:** "Find me recent news on AI"
- Results: Random Chrome updates, Oklahoma data centers, vague healthcare advances
- No date specificity, basically useless

**Amazing Query:** "Find me diverse, well-grounded novel AI updates since [specific date] focused on the build use case. Surprise me."
- Results: Specific product releases with dates, API access updates, regional trends
- Led to fascinating discoveries and productive follow-up questions

## Key Philosophy

Perplexity isn't the awkward middle ground between Google and ChatGPT - it's a fundamentally different tool for internet-native research. Use it when you need:

- Current, sourced, verifiable information
- Transparency in sources
- Accountability in claims
- Real-time web knowledge instead of training data

Remember: Perplexity says "These sources claim this. Here are the sources. You decide." - not "I believe this based on patterns."
