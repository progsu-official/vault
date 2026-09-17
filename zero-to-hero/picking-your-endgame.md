---
title: "Picking your endgame"
author:
  name: "progsu team"
  handle: "@progsu"
readTime: "9 min read"
publishDate: 2026-08-02T00:00:00.000Z
updated: 2026-08-22T00:00:00.000Z
tags: [career, roadmap, compensation, role-selection]
category: zero-to-hero
---

# picking your endgame

[[getting-started]] told you to reverse engineer your roadmap from the destination. this is where you pick the destination.

five tracks get covered here = software engineering, AI/ML, quant dev, data, and cybersecurity. for each one we go through what the market pays, what the day-to-day actually looks like, and what it costs to get in. none of these picks are permanent, so don't stay stagnant. as long as you keep moving and stay in motion, you can still change and correct course. that beats staying undecided for three years, because an undecided roadmap produces undecided reps.

## the roadmap

start with the technical map for the track you're eyeing. [roadmap.sh](https://roadmap.sh) publishes a maintained skill tree for most of them:

- **software engineering**: [backend](https://roadmap.sh/backend), [frontend](https://roadmap.sh/frontend), or [full stack](https://roadmap.sh/full-stack)
- **AI/ML**: [ai engineer](https://roadmap.sh/ai-engineer) for the applied side, [ai and data scientist](https://roadmap.sh/ai-data-scientist) for research
- **data**: [data analyst](https://roadmap.sh/data-analyst). add [backend](https://roadmap.sh/backend) if you're moving toward data engineering
- **cybersecurity**: [cybersecurity](https://roadmap.sh/cyber-security)
- **quant dev**: no dedicated roadmap. it's the CS core plus probability, statistics, and linear algebra, with C++ or Python depth on top

skim the [computer science](https://roadmap.sh/computer-science) roadmap too. it's the shared base under all five.

> [!note]
> roadmap.sh tells you what to learn. whether you want the job is a separate question. that's the rest of this page.

## macro vs micro

every track gets judged on two questions. most people only ask one.

**macro** is the market question = what does this field pay, how many seats exist, how safe are they. **micro** is the fit question = what does the work feel like day to day, and would you still want it in a decade.

ask only the macro question and you grind toward a number you'll quit two years in. ask only the micro question and you fall for a role with fifty openings a year in three cities. both have to hold.

### macro, the market view

entry-level total compensation in the US, mid 2026. total comp means base plus bonus plus equity all added together.

| track | 25th | median | 75th |
|---|---|---|---|
| software engineering | $85k | $115k | $175k |
| AI/ML | $110k | $150k | $220k |
| quant dev | $175k | $250k | $350k+ |
| data | $70k | $95k | $130k |
| cybersecurity | $65k | $85k | $115k |

the spread inside a track matters more than the gap between tracks. a big tech SWE offer clears $180k. a local shop offers $75k for the same title the same year. that gap comes down to which company you picked, so it's a company-selection problem.

| track | senior ceiling | seats at entry | Atlanta |
|---|---|---|---|
| software engineering | $250k to $500k+ | largest, most contested | strong |
| AI/ML | $300k to $800k+ | growing fast, thin at entry | thin at entry |
| quant dev | $500k to $1m+ | a few hundred a year, nationally | basically none |
| data | $180k to $300k | large, widest entry door | strong |
| cybersecurity | $180k to $280k | growing, blue team is the entry door | strong |

> [!warning]
> these numbers are a snapshot. check [levels.fyi](https://levels.fyi) before deciding anything on them. treat any figure older than a year as directional.

a few things to read off those tables. quant dev pays the most and is the hardest seat to get, so treating it as a fallback is a mistake. AI/ML pays well but hires thin at entry, since most openings want a master's or real research output. that makes it a better second job than first job. data and blue team cybersecurity have the lowest ceilings and the widest doors, which makes them the most reliable way in when SWE applications stall.

job security tracks with how boring the work sounds. security operations, internal tooling, data pipelines, payments infrastructure. all unglamorous, and all extremely hard to cut, because something breaks the moment they stop. the roles closest to a company's discretionary spending are the ones that get cut first.

> [!note] note on Atlanta
> the local market is real but uneven. software engineering and data hire steadily across logistics, healthcare, and the big local employers. Atlanta is also a genuine payments and fintech hub, which makes it one of the strongest blue team markets in the country. quant dev is the exception, since those desks live in New York and Chicago. that endgame means relocating. see [[local-atl-resources]] for the local scene.

### micro, the day-to-day view

comp gets you in the door. this is the work once you're through it.

- **software engineering.** most of the day goes into reading existing code, and writing new code is the smaller half. you pick up a ticket, trace how the system handles it now, make a change, then defend it in review. good fit if you like building and can sit with ambiguity before anything works. core skills = one language deeply, data structures and algorithms, git, and enough systems knowledge to reason about what's slow.
- **AI/ML.** two very different jobs share the label. AI engineering is software engineering pointed at models = pipelines, evals, serving, integration. research is closer to grad school, so reading papers and running experiments that mostly fail. good fit if you like math and can be wrong most of the week. core skills = Python, linear algebra, probability, and experiment discipline.
- **quant dev.** you either trade live markets, research signals, or build the low-latency systems underneath both. feedback loops are short and everything gets measured against a number. good fit if you like competition and think clearly under live pressure. core skills = probability, statistics, mental math, and C++ or Python depth. the interview bar is the real filter, see [[dsa-leetcode-strategy]].
- **data.** you turn messy real-world data into something a decision can rest on = SQL, pipelines, dashboards. half the job is conversations with people who aren't technical. good fit if you like answering questions with evidence. core skills = SQL fluency first, then Python, then warehousing and orchestration tools.
- **cybersecurity, blue team.** defensive security. you watch alerts, investigate whether something is a real intrusion or just noise, harden systems, then write the detection that catches it next time. investigative work with heavy on-call. good fit if you're curious, patient, and calm while something is actively going wrong. core skills = networking, operating systems, log analysis, and scripting. certifications carry real weight here, unlike in the other four.

once you're in, comp grows three ways, and each track favors a different one.

- **job hopping.** the fastest lever early. a move every two to three years beats an internal raise. it works best in software engineering and data, where the market is deep.
- **climbing the ladder.** slower, and the curve steepens later. senior to staff is where those ceiling numbers come from. quant dev compresses the timeline hard, so first-year bonuses can rival a senior SWE salary.
- **starting a company.** highest variance by a wide margin. treat it as a post-experience move. the tracks that prepare you best are the ones where you shipped user-facing product.

## what this actually takes

comp and day-to-day are the reward side. this is what it costs.

| track | credentials | typical hours | who it suits |
|---|---|---|---|
| software engineering | BS is enough | 40 to 50 | builders, tolerant of ambiguity |
| AI/ML | MS or PhD for research | 45 to 55 | mathematically curious |
| quant dev | BS, but a brutal interview bar | 50 to 60+ | competitive, calm under pressure |
| data | BS plus SQL and a portfolio | 40 to 45 | evidence-driven communicators |
| cybersecurity | BS plus certifications | 40 to 50, plus on-call | patient investigators |

**short-term effort** is the same everywhere = a finished project, real interview preparation, and a resume that survives a follow-up question. that baseline holds across all five tracks, so start it before you've decided. [[landing-your-first-internship]] covers the sequence.

**long-term effort** is where the tracks separate. software engineering and data stay sustainable, since the skills compound and the pace is human. AI/ML research asks for years of formal education before the interesting work starts. quant dev demands the heaviest sustained intensity, and the comp exists partly because most people quit that pace inside ten years. cybersecurity asks for continuous recertification and a tolerance for your phone going off at 3am.

**credentials** genuinely gate two of these. AI/ML research effectively requires a graduate degree. cybersecurity hiring leans on certifications harder than any other track, and that's exactly what makes blue team a viable entry path, since a certification is a few months of study instead of a few years of school. everywhere else, a bachelor's plus proof you can build is the whole requirement.

**work-life balance** is a company property more than a track property, and quant dev is the honest exception. a startup SWE role can be harder than a quant dev seat. a mature enterprise data role can be easier than either. so ask about hours during interviews, and weight what current employees say over what the recruiter says.

**personality fit** is the one nobody audits honestly, and it also decides whether you're still here in five years. if reading someone else's code all day sounds miserable, software engineering stays exactly that. if ambiguity stresses you out, research stays ambiguous forever. pick the day-to-day you can stand on a bad week, because the one that sounds best out loud is a different question entirely.

## where to go next

- [[getting-started]], for the overall roadmap and how to reverse engineer backward from whatever you picked here
- [[roadmap-by-year]], to see what your chosen track should look like at your current stage
- [[landing-your-first-internship]], for the search playbook once you have a direction
- [[building-experience-early]], if you're early and need experience before any of this applies

## turn this into action

pick one track and one backup before you close this tab. then find three entry-level postings in that track and read the requirements closely. the gap between those requirements and your current resume is your roadmap for the next year. the market wrote it, so you don't have to.

if nothing here felt like an obvious yes, pick anyway and default to software engineering. it's the widest door and the most transferable skill set, and every other track on this list is reachable from it later.
