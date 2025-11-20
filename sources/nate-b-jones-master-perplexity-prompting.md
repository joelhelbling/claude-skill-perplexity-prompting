# Master Perplexity Prompting -- Why It's Different from ChatGPT + Demo

_A summary from [Nate B. Jones' Youtube video](https://www.youtube.com/watch?v=05RRGiF7QC0)._

## What Makes Perplexity Different from Everything Else

• **Perplexity is NOT Google or ChatGPT** - It's an AI-native search engine that uses something called "retrieval augmented generation" (RAG)
• **How it works**: Takes your question → searches the entire internet → finds relevant documents → extracts key info → crafts an answer with citations
• **Research Mode is INSANE**: Does dozens of searches, reads hundreds of sources, and makes multiple passes to find the absolute best answer (like turning the effort dial to 11!)

• **ChatGPT vs Perplexity - The Big Difference**:
  - ChatGPT = looks inside its own brain (training data) first
  - Perplexity = looks at the whole internet first
  - That's why ChatGPT doesn't even know what the current ChatGPT model is! It's looking inward, not outward

## The 8 Non-Obvious Prompting Strategies That Will Blow Your Mind

### 1. A Little Goes a Long Way
• Just 2-3 words of context can DRAMATICALLY improve results
• **Bad**: "climate models" 
• **Good**: "climate prediction models for urban planning"
• Perplexity prompts are actually SHORTER than ChatGPT prompts on average!

### 2. NEVER Use Few-Shot Prompting (This is Huge!)
• Don't give examples like you would with ChatGPT
• **Why**: Perplexity will obsess over your examples and only find similar things
• **Example**: Say "French architecture like the Louvre" and you'll ONLY get museums, nothing else about French architecture

### 3. Use Exact Search Parameters
• Be specific about things Perplexity is built to understand:
  - "Filter by sources from 2024" instead of "recent sources"
  - "Limit to 5 academic sources"
  - "Search depth: comprehensive"
• The more specific you are about dates/sources, the better quality you get

### 4. Demand Multiple Perspectives
• **Instead of**: "What are health benefits of X?"
• **Do this**: "Compare findings from at least three peer-reviewed studies on X and note conflicts in conclusions"
• This forces triangulation instead of just parroting one source

### 5. Progressive Deepening (The Conversation Technique)
• Start BROADER than you would with ChatGPT
• Let each answer open up new questions
• Thread through the conversation to drill down
• First query maps the territory, then you explore promising paths
• **This is totally different from ChatGPT** where you want everything structured upfront

### 6. Specify Output Constraints to Reduce Hallucinations
• **Example**: "Provide evidence for every claim with specific section references and page numbers so I can check your work"
• Forces Perplexity to verify at a granular level instead of making broad assumptions

### 7. Strategic Focus Mode Usage
• Use Academic mode for peer-reviewed sources
• Use Social mode for social media insights
• **Pro tip**: Switch modes MID-CONVERSATION to reset the model's thinking without losing context
• This is different from ChatGPT where you'd need to start over completely

### 8. Create Custom Spaces for Repeated Workflows
• Upload reference files and set standing instructions
• **Example**: Competitive intelligence space with instruction "Structure all responses as: current state, competitive positioning, emerging threats, strategic implications"
• Perfect for internet-first projects like stock analysis, news monitoring, financial research

## Real Example: Bad vs. Amazing Search

### Bad Search: "Find me recent news on AI"
• Got random stuff like Chrome updates mixed with Oklahoma data centers
• Vague healthcare advances
• No date specificity
• Basically useless

### Amazing Search: "Find me diverse, well-grounded novel AI updates since [specific date] focused on the build use case. Surprise me."
• Got Agent Kit updates with date caveats
• GPT-5 Pro availability
• Sora 2 API access
• Anthropic's coding push
• Discovered Korean Claude Code culture (who knew?!)
• Led to fascinating follow-up about AI build culture in Korea

## How to Avoid Hallucinations (Critical!)

### Red Flags to Watch For:
• **Single source answers** - especially from random blogs or LinkedIn posts
• **AI-generated spam** - Perplexity can't tell the difference between real and AI content
• **Quote attribution issues** - always check the actual source for exact wording and context

### Protection Strategies:
• **Use academic focus mode** for authoritative sources (prioritizes PubMed, Semantic Scholar)
• **Double-check with another LLM** - use ChatGPT to verify Perplexity results and vice versa
• **Verify links manually** - not all "verified" links actually work
• **Cross-reference multiple sources** before trusting any claim

## Why Perplexity Matters in an AI World

### The Knowledge Recency Problem
• LLM training data gets outdated too fast
• AI knowledge is expanding rapidly
• Perplexity updates its knowledge base multiple times daily
• ChatGPT treats current info as separate from its core model

### Accountability Architecture
• Everything is sourced and transparent
• You can see and evaluate every source
• Creates "verifiable chains of reasoning"
• Unlike LLMs that just say "I believe this based on patterns"

### Different Epistemological Approaches (Fancy but Important!)
• **ChatGPT**: "I believe this is true based on patterns" (leads to confident-sounding hallucinations)
• **Perplexity**: "These sources claim this. Here are the sources. You decide."
• As AI gets more fluent, the gap between sounding smart and being factual widens
• Perplexity gives us an AI-native way to check facts, not just patterns

## Best Use Cases for Perplexity
• Competitive intelligence
• Stock and financial analysis  
• Breaking news and current events
• Academic research with recent developments
• Discovering unexpected connections (like Korean Claude Code culture!)
• Any situation where you need internet-first, up-to-date information

## Key Takeaway
Perplexity isn't the awkward middle ground between Google and ChatGPT - it's a fundamentally different tool that excels at internet-native research and discovery. Use it when you need current, sourced, verifiable information that you can actually check!
