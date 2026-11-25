# Jadeline

**AI deal intelligence for Asian venture investors.**
Human judgement, amplified and justified.

Prototype: https://jadeline.vercel.app

## The problem
Early stage investors in Southeast Asia and India still benchmark deals mostly from memory and personal networks. Public data is thin, US benchmarks don't fit, and most tools focus on finding companies, not on deciding whether a deal is worth it. It is "Human judgement, amplified and justified by Jadeline"

## What Jadeline does
1. **Scores a Seed to Series C deal** on four pillars: market and product market fit, unit economics, the ask, and the founders. Every score shows the rule and peer set behind it.
2. **Simulates returns** from the investor's own deployment path (cheque, reserves, follow on choices) through later rounds to IPO, trade sale or write off, across 5,000 simulated futures. Results are ranges, never single numbers.
3. **Adapts to each firm.** A firm can override any assumption and see its own view next to the market baseline, with each firm's data kept private by database level security.

## Built on real data
Benchmarks come from primary sources: IPO prospectuses and SEC filings, read with Claude and confirmed by an analyst. Each figure keeps its source, quote and sample size. The truth set currently covers Sea, Grab and Honasa, with Zomato, Nykaa, PB Fintech, Delhivery and Swiggy in review.

Odds of raising the next round come from cited industry sources rather than from listed companies, so the model isn't fooled by survivorship bias.

## Stack
Next.js and TypeScript, Supabase (Postgres with row level security), a Python returns engine (FastAPI, numpy), and the Claude API for document extraction. Hundreds of automated tests, including hand checked cases for the returns maths.

## Status
In active development: Singapore and Southeast Asia first, India second. Built by Sambhav Jain with Claude Code.

Full source code available on request.
