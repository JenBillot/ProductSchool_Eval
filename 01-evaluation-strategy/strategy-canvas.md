# AI Evaluation Strategy Canvas

> Repo file `ai-evals/01-evaluation-strategy/strategy-canvas.md` (the repo is your submission).
> Becomes the Strategy Canvas slide of the final pitch deck you assemble in Module 6.

## 1. Product Strategy, The Context

**Target user:** VP-level Strategists and Product Leaders at Fortune 500 companies who pay a premium for verified market intelligence and want access to our premium B2B market-intelligence platform.   On average they pay at least $50k+ annually for verified data to inform their roadmaps.

**Key use case:** They want to quickly get access to market intelligence (like market share for start ups to inform purchasing decisions, or understand competitors focus areas et) so that the users can update their roadmaps to maintain/gain market share and differentiate their offering 

**Value proposition:** Users are willing to pay an annual fee to get personalized responseso on market intelligence insights that are instant. The responses are based on verified data and up to date information. The benefit is the tool should significantly reduce the time spent searching for market insights 

## 2. Measurements, The Execution

**User promise.** For VP-level Enterprise Strategists, Ascend IQ promises to deliver accurate, verified, citation-backed competitive intelligence in under 5 seconds so that they can develop their roadmaps that drive the business objectives (i.e. market share) 

**Top 3 trust metrics:**
- **Latency**, Response speed (P95 / P99). Slow kills engagement.
- **Hallucination Rate**, % of outputs that are confidently false or fabricated.
- **Robustness**, Coherence on messy, adversarial, out-of-scope inputs.

**Why these three:** • Hallucination, VP-level clients pay $50k+ for verified data therefore it's crucial that it is verified and not falsified 
• Latency; Users have told us that results are taking too long which needs to be improved 
• Robustness; Rolling out to 50 Enterprise accounts means messy, unpredictable real-world queries will hit the system at scale, and a confidently wrong or broken response to an edge case destroys trust faster than a slow one ever could

## 3. Strategic Trade-Offs, The Cost

### Trade-off 1 · Hallucination Rate ↔ Latency
We prioritize Hallucination Rate over Robustness because a visible "I don't know" preserves trust, but a confident fabrication can silently drive a $1M decision.

### Trade-off 2 · Latency ↔ Robustness
We prioritize Robustness over Latency because a broken response to a messy query loses a VP's trust for good, while a few extra seconds of validation is barely noticed.

---
_Generated from the AI Evaluation Strategy Canvas, M1 lab tool, AI Evals Certification._
