# CoCo Hackathon Bootstrap Kit

This kit gives you a structured starting point for building with Cortex Code (CoCo) during a hackathon. Whether you're a seasoned engineer or picking up an AI coding assistant for the first time, the templates and guardrails here are designed to keep you moving toward a working demo — not a perfect codebase. Use the plan, follow the phases, and let CoCo handle the implementation details.

## What's in This Kit

| File | What it does |
|------|--------------|
| `AGENTS.md` | Configures CoCo's behavior for your project. Drop it in your project root. |
| `PLAN_template.md` | Phased execution plan. Copy, rename, fill in the blanks, and go. |
| `skill/SKILL.md` | Interactive hackathon coach. Invoke with `$hackathon-coach` in any CoCo session. |
| `plans/` | Where your project plan lives after you copy `PLAN_template.md` here. |

## Quick Start (5 minutes)

1. Copy this entire folder into your project root
2. Open a CoCo session in your project directory
3. Type: `$hackathon-coach` and answer the setup questions
4. CoCo will create a customized plan for your use case in `plans/`
5. Follow Phase 0 in your plan — you're off

## Using CoCo Effectively

### Beginner Tips

> - CoCo is a conversation. Talk to it like a senior developer on your team.
> - Be specific: "Build me a Streamlit app that shows patient counts by region using Snowflake" beats "make an app"
> - If it goes off track, just say "stop — let's back up" and redirect
> - Use `$hackathon-coach` at any point if you feel lost — it'll re-orient you

### Engineer Tips

> - `AGENTS.md` is your system prompt — edit it to match your preferences
> - `cortex ctx remember` is your persistent memory — save key decisions so they survive context resets
> - Use phases as guardrails, not rigid gates — skip or compress phases if you're moving fast
> - For Snowflake work: Cortex AI Functions (`AI_COMPLETE`, `AI_CLASSIFY`, `AI_EXTRACT`), Semantic Views, and Dynamic Tables are your highest-leverage primitives

## The CoCo Mindset

- CoCo works best when you have a clear goal and let it handle implementation details
- The plan is the contract — keep it updated and CoCo stays oriented
- Validation gates exist so you don't discover broken foundations in Phase 4
- "Done" at a hackathon means: works in the demo, tells a story, shows the Snowflake value

## Snowflake Features to Know

| Feature | Best for | How to ask CoCo |
|---------|----------|-----------------|
| Cortex AI Functions (`AI_COMPLETE`, `AI_CLASSIFY`, `AI_EXTRACT`, `AI_SUMMARIZE`) | Text analysis, classification, extraction | "Use AI_CLASSIFY to tag these records by category" |
| Cortex Agents | Multi-step reasoning with tool use | "Build a Cortex Agent that answers questions about my data" |
| Streamlit in Snowflake | Interactive data apps | "Build a Streamlit app that connects to my Snowflake table" |
| Dynamic Tables | Auto-refreshing pipelines | "Create a dynamic table that refreshes my aggregations every hour" |
| Semantic Views | Natural language querying | "Create a semantic view so users can ask questions in plain English" |
| Snowpark Python | Custom Python logic in Snowflake | "Write a Snowpark UDF that scores these records" |
| Cortex Search | Search over unstructured data | "Set up a Cortex Search service over my documents table" |

## Phase Time Guide

| Phase | 4-hour event | 6-hour event |
|-------|-------------|-------------|
| 0 — Orient & Setup | 15 min | 15 min |
| 1 — Requirements & Architecture | 20 min | 25 min |
| 2 — Scaffold & Stub | 30 min | 40 min |
| 3 — Core Build | 90 min | 150 min |
| 4 — Polish & Demo Prep | 25 min | 35 min |
| Buffer | 0 min | 15 min |

## Getting Help

- Invoke the coach: `$hackathon-coach`
- Check your plan: `cortex ctx show tasks`
- Save a decision: `cortex ctx remember "I chose Streamlit because..."`
- If CoCo loses context: re-run `$hackathon-coach` and tell it which phase you're in

---

Built for Snowflake SE team hackathon enablement. Maintained by Braedon Hill, Sr. Solution Engineer.
