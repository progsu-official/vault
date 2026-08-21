---
title: "Picking your endgame: industry, role, lifestyle"
author:
  name: "progsu team"
  handle: "@progsu"
readTime: "7 min read"
publishDate: 2026-08-02T00:00:00.000Z
updated: 2026-08-20T00:00:00.000Z
tags: [career, roadmap, compensation, role-selection]
category: zero-to-hero
---

# picking your endgame: industry, role, lifestyle

[[getting-started]] told you to reverse engineer your roadmap from the destination. This is where you pick the destination.

Five tracks get covered here: software engineering, ai/ml, quant, data, and cybersecurity. For each one: what the market pays, what the work feels like on a random tuesday, and what it costs to get in. Every one of these is reversible. Pick a direction now and correct in a year. That beats staying undecided for three, because an undecided roadmap produces undecided reps.

## the roadmap

Start with the technical map for the track you're eyeing. [roadmap.sh](https://roadmap.sh) publishes a maintained skill tree for most of them:

- **software engineering**: [backend](https://roadmap.sh/backend), [frontend](https://roadmap.sh/frontend), or [full stack](https://roadmap.sh/full-stack)
- **ai/ml**: [ai engineer](https://roadmap.sh/ai-engineer) for the applied side, [ai and data scientist](https://roadmap.sh/ai-data-scientist) for research
- **data**: [data analyst](https://roadmap.sh/data-analyst). Add [backend](https://roadmap.sh/backend) if you're moving toward data engineering
- **cybersecurity**: [cyber security](https://roadmap.sh/cyber-security)
- **quant**: no dedicated roadmap. It's the cs core plus probability, statistics, and linear algebra, with c++ or python depth on top

Skim the [computer science](https://roadmap.sh/computer-science) roadmap too. It's the shared base under all five.

> **note:** roadmap.sh tells you what to learn. Whether you want the job is a separate question. That's the rest of this page.

## macro vs micro

Every track gets judged on two questions. Most people only ask one.

**Macro** is the market question: what does this field pay, how many seats exist, how safe are they. **Micro** is the fit question: what does the work feel like day to day, and would you still want it in a decade.

Ask only the macro question and you grind toward a number you'll quit two years in. Ask only the micro question and you fall for a role with fifty openings a year in three cities. Both have to hold.

### macro: the market view

Entry-level total compensation in the us, mid 2026. Total comp means base plus bonus plus equity, not base alone.

| track | 25th | median | 75th |
|---|---|---|---|
| software engineering | $85k | $115k | $175k |
| ai/ml | $110k | $150k | $220k |
| quant | $175k | $250k | $350k+ |
| data | $70k | $95k | $130k |
| cybersecurity | $65k | $85k | $115k |

The spread inside a track matters more than the gap between tracks. A big tech swe offer clears $180k. A local shop offers $75k for the same title the same year. That gap is company selection, not career selection.

| track | senior ceiling | seats at entry | atlanta |
|---|---|---|---|
| software engineering | $250k to $500k+ | largest, most contested | strong |
| ai/ml | $300k to $800k+ | growing fast, thin at entry | thin at entry |
| quant | $500k to $1m+ | a few hundred a year, nationally | essentially none |
| data | $180k to $300k | large, widest entry door | strong |
| cybersecurity | $180k to $280k | growing, blue team is the entry door | strong |

A few things to read off those tables. Quant pays the most and is the hardest seat to get. Treating it as a fallback is a mistake. Ai/ml pays well but hires thin at entry, since most openings want a masters or real research output. It makes a better second job than first job. Data and blue team cybersecurity have the lowest ceilings and the widest doors. That makes them the most reliable way in when swe applications stall.

Job security tracks with how boring the work sounds. Security operations, internal tooling, data pipelines, payments infrastructure. All unglamorous. All extremely hard to cut, because something breaks the moment they stop. Roles closest to a company's discretionary spending get cut first.

> **note on atlanta:** the local market is real but uneven. Software engineering and data hire steadily across logistics, healthcare, and the big local employers. Atlanta is also a genuine payments and fintech hub. That makes it one of the strongest blue team markets in the country. Quant is the exception, those desks live in new york and chicago. That endgame means relocating. See [[local-atl-resources]] for the local scene.

> **warning:** these numbers are a snapshot. Check [levels.fyi](https://levels.fyi) before deciding anything on them. Treat any figure older than a year as directional.

### micro: the day-to-day view

Comp gets you in the door. This is the work once you're through it.

- **software engineering.** Most of the day is reading existing code, not writing new code. You pick up a ticket, trace how the system handles it now, make a change, then defend it in review. Good fit if you like building and can sit with ambiguity before anything works. Core skills: one language deeply, data structures and algorithms, git, and enough systems knowledge to reason about what's slow.
- **ai/ml.** Two very different jobs share the label. Ai engineering is software engineering pointed at models: pipelines, evals, serving, integration. Research is closer to grad school, reading papers and running experiments that mostly fail. Good fit if you like math and can be wrong most of the week. Core skills: python, linear algebra, probability, and experiment discipline.
- **quant.** You either trade live markets, research signals, or build the low-latency systems underneath both. Feedback loops are short. Everything gets measured against a number. Good fit if you like competition and think clearly under live pressure. Core skills: probability, statistics, mental math, and c++ or python depth. The interview bar is the real filter, see [[dsa-leetcode-strategy]].
- **data.** You turn messy real-world data into something a decision can rest on: sql, pipelines, dashboards. Half the job is conversations with people who aren't technical. Good fit if you like answering questions with evidence. Core skills: sql fluency first, then python, then warehousing and orchestration tools.
- **cybersecurity, blue team.** Defensive security. You watch alerts, investigate whether something is a real intrusion or noise, harden systems, then write the detection that catches it next time. Investigative work with heavy on-call. Good fit if you're curious, patient, and calm while something is actively going wrong. Core skills: networking, operating systems, log analysis, and scripting. Certifications carry real weight here, unlike in the other four.

Once you're in, comp grows three ways. Each track favors a different one.

- **job hopping.** The fastest lever early. A move every two to three years beats an internal raise. It works best in software engineering and data, where the market is deep.
- **climbing the ladder.** Slower, and the curve steepens later. Senior to staff is where those ceiling numbers come from. Quant compresses the timeline hard, first-year bonuses can rival a senior swe salary.
- **starting a company.** Highest variance by a wide margin. Treat it as a post-experience move. The tracks that prepare you best are the ones where you shipped user-facing product.

## what does this actually take?

Comp and day-to-day are the reward side. This is the bill.

| track | credentials | typical hours | who it suits |
|---|---|---|---|
| software engineering | bs is enough | 40 to 50 | builders, tolerant of ambiguity |
| ai/ml | ms or phd for research | 45 to 55 | mathematically curious |
| quant | bs, but a brutal interview bar | 50 to 60+ | competitive, calm under pressure |
| data | bs plus sql and a portfolio | 40 to 45 | evidence-driven communicators |
| cybersecurity | bs plus certifications | 40 to 50, plus on-call | patient investigators |

**Short-term effort** is the same everywhere: a finished project, real interview preparation, and a resume that survives a follow-up question. That baseline holds across all five tracks. Start it before you've decided. [[landing-your-first-internship]] covers the sequence.

**Long-term effort** is where the tracks separate. Software engineering and data stay sustainable, the skills compound and the pace is human. Ai/ml research asks for years of formal education before the interesting work starts. Quant demands the heaviest sustained intensity. The comp exists partly because most people quit that pace inside ten years. Cybersecurity asks for continuous recertification and a tolerance for your phone going off at 3am.

**Credentials** genuinely gate two of these. Ai/ml research effectively requires a graduate degree. Cybersecurity hiring leans on certifications harder than any other track. That's exactly what makes blue team a viable entry path: a certification is a few months of study, not a few years of school. Everywhere else, a bachelors plus proof you can build is the whole requirement.

**Work-life balance** is a company property more than a track property. Quant is the honest exception. A startup swe role can be harder than a quant seat. A mature enterprise data role can be easier than either. Ask about hours during interviews. Weight what current employees say over what the recruiter says.

**Personality fit** is the one nobody audits honestly. It also decides whether you're still here in five years. If reading someone else's code all day sounds miserable, software engineering stays exactly that. If ambiguity stresses you out, research stays ambiguous forever. Pick the day-to-day you can stand on a bad week, not the one that sounds best out loud.

## where to go next

- [[getting-started]], for the overall roadmap and how to reverse engineer backward from whatever you picked here
- [[roadmap-by-year]], to see what your chosen track should look like at your current stage
- [[landing-your-first-internship]], for the search playbook once you have a direction
- [[building-experience-early]], if you're early and need experience before any of this applies

## turn this into action

Pick one track and one backup before you close this tab. Then find three entry-level postings in that track and read the requirements closely. The gap between those requirements and your current resume is your roadmap for the next year. The market wrote it, so you don't have to.

If nothing here felt like an obvious yes, pick anyway. Default to software engineering. It's the widest door and the most transferable skill set. Every other track on this list is reachable from it later.
