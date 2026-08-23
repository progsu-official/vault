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

[[getting-started]] told you to reverse engineer your roadmap from the destination. This is where you pick the destination.

Five tracks get covered here = software engineering, AI/ML, quant dev, data, and cybersecurity. For each one we go through what the market pays, what the day-to-day actually looks like, and what it costs to get in. None of these picks are permanent, so don't stay stagnant. As long as you keep moving and stay in motion, you can still change and correct course. That beats staying undecided for three years, because an undecided roadmap produces undecided reps.

## the roadmap

Start with the technical map for the track you're eyeing. [roadmap.sh](https://roadmap.sh) publishes a maintained skill tree for most of them:

- **software engineering**: [backend](https://roadmap.sh/backend), [frontend](https://roadmap.sh/frontend), or [full stack](https://roadmap.sh/full-stack)
- **AI/ML**: [ai engineer](https://roadmap.sh/ai-engineer) for the applied side, [ai and data scientist](https://roadmap.sh/ai-data-scientist) for research
- **data**: [data analyst](https://roadmap.sh/data-analyst). Add [backend](https://roadmap.sh/backend) if you're moving toward data engineering
- **cybersecurity**: [cybersecurity](https://roadmap.sh/cyber-security)
- **quant dev**: no dedicated roadmap. It's the CS core plus probability, statistics, and linear algebra, with C++ or Python depth on top

Skim the [computer science](https://roadmap.sh/computer-science) roadmap too. It's the shared base under all five.

> [!note]
> roadmap.sh tells you what to learn. Whether you want the job is a separate question. That's the rest of this page.

## macro vs micro

Every track gets judged on two questions. Most people only ask one.

**Macro** is the market question = what does this field pay, how many seats exist, how safe are they. **Micro** is the fit question = what does the work feel like day to day, and would you still want it in a decade.

Ask only the macro question and you grind toward a number you'll quit two years in. Ask only the micro question and you fall for a role with fifty openings a year in three cities. Both have to hold.

### macro, the market view

Entry-level total compensation in the US, mid 2026. Total comp means base plus bonus plus equity all added together.

| track | 25th | median | 75th |
|---|---|---|---|
| software engineering | $85k | $115k | $175k |
| AI/ML | $110k | $150k | $220k |
| quant dev | $175k | $250k | $350k+ |
| data | $70k | $95k | $130k |
| cybersecurity | $65k | $85k | $115k |

The spread inside a track matters more than the gap between tracks. A big tech SWE offer clears $180k. A local shop offers $75k for the same title the same year. That gap comes down to which company you picked, so it's a company-selection problem.

| track | senior ceiling | seats at entry | Atlanta |
|---|---|---|---|
| software engineering | $250k to $500k+ | largest, most contested | strong |
| AI/ML | $300k to $800k+ | growing fast, thin at entry | thin at entry |
| quant dev | $500k to $1m+ | a few hundred a year, nationally | basically none |
| data | $180k to $300k | large, widest entry door | strong |
| cybersecurity | $180k to $280k | growing, blue team is the entry door | strong |

> [!warning]
> These numbers are a snapshot. Check [levels.fyi](https://levels.fyi) before deciding anything on them. Treat any figure older than a year as directional.

A few things to read off those tables. Quant dev pays the most and is the hardest seat to get, so treating it as a fallback is a mistake. AI/ML pays well but hires thin at entry, since most openings want a master's or real research output. That makes it a better second job than first job. Data and blue team cybersecurity have the lowest ceilings and the widest doors, which makes them the most reliable way in when SWE applications stall.

Job security tracks with how boring the work sounds. Security operations, internal tooling, data pipelines, payments infrastructure. All unglamorous, and all extremely hard to cut, because something breaks the moment they stop. The roles closest to a company's discretionary spending are the ones that get cut first.

> [!note] note on Atlanta
> The local market is real but uneven. Software engineering and data hire steadily across logistics, healthcare, and the big local employers. Atlanta is also a genuine payments and fintech hub, which makes it one of the strongest blue team markets in the country. Quant dev is the exception, since those desks live in New York and Chicago. That endgame means relocating. See [[local-atl-resources]] for the local scene.

### micro, the day-to-day view

Comp gets you in the door. This is the work once you're through it.

- **software engineering.** Most of the day goes into reading existing code, and writing new code is the smaller half. You pick up a ticket, trace how the system handles it now, make a change, then defend it in review. Good fit if you like building and can sit with ambiguity before anything works. Core skills = one language deeply, data structures and algorithms, git, and enough systems knowledge to reason about what's slow.
- **AI/ML.** Two very different jobs share the label. AI engineering is software engineering pointed at models = pipelines, evals, serving, integration. Research is closer to grad school, so reading papers and running experiments that mostly fail. Good fit if you like math and can be wrong most of the week. Core skills = Python, linear algebra, probability, and experiment discipline.
- **quant dev.** You either trade live markets, research signals, or build the low-latency systems underneath both. Feedback loops are short and everything gets measured against a number. Good fit if you like competition and think clearly under live pressure. Core skills = probability, statistics, mental math, and C++ or Python depth. The interview bar is the real filter, see [[dsa-leetcode-strategy]].
- **data.** You turn messy real-world data into something a decision can rest on = SQL, pipelines, dashboards. Half the job is conversations with people who aren't technical. Good fit if you like answering questions with evidence. Core skills = SQL fluency first, then Python, then warehousing and orchestration tools.
- **cybersecurity, blue team.** Defensive security. You watch alerts, investigate whether something is a real intrusion or just noise, harden systems, then write the detection that catches it next time. Investigative work with heavy on-call. Good fit if you're curious, patient, and calm while something is actively going wrong. Core skills = networking, operating systems, log analysis, and scripting. Certifications carry real weight here, unlike in the other four.

Once you're in, comp grows three ways, and each track favors a different one.

- **job hopping.** The fastest lever early. A move every two to three years beats an internal raise. It works best in software engineering and data, where the market is deep.
- **climbing the ladder.** Slower, and the curve steepens later. Senior to staff is where those ceiling numbers come from. Quant dev compresses the timeline hard, so first-year bonuses can rival a senior SWE salary.
- **starting a company.** Highest variance by a wide margin. Treat it as a post-experience move. The tracks that prepare you best are the ones where you shipped user-facing product.

## what this actually takes

Comp and day-to-day are the reward side. This is what it costs.

| track | credentials | typical hours | who it suits |
|---|---|---|---|
| software engineering | BS is enough | 40 to 50 | builders, tolerant of ambiguity |
| AI/ML | MS or PhD for research | 45 to 55 | mathematically curious |
| quant dev | BS, but a brutal interview bar | 50 to 60+ | competitive, calm under pressure |
| data | BS plus SQL and a portfolio | 40 to 45 | evidence-driven communicators |
| cybersecurity | BS plus certifications | 40 to 50, plus on-call | patient investigators |

**Short-term effort** is the same everywhere = a finished project, real interview preparation, and a resume that survives a follow-up question. That baseline holds across all five tracks, so start it before you've decided. [[landing-your-first-internship]] covers the sequence.

**Long-term effort** is where the tracks separate. Software engineering and data stay sustainable, since the skills compound and the pace is human. AI/ML research asks for years of formal education before the interesting work starts. Quant dev demands the heaviest sustained intensity, and the comp exists partly because most people quit that pace inside ten years. Cybersecurity asks for continuous recertification and a tolerance for your phone going off at 3am.

**Credentials** genuinely gate two of these. AI/ML research effectively requires a graduate degree. Cybersecurity hiring leans on certifications harder than any other track, and that's exactly what makes blue team a viable entry path, since a certification is a few months of study instead of a few years of school. Everywhere else, a bachelor's plus proof you can build is the whole requirement.

**Work-life balance** is a company property more than a track property, and quant dev is the honest exception. A startup SWE role can be harder than a quant dev seat. A mature enterprise data role can be easier than either. So ask about hours during interviews, and weight what current employees say over what the recruiter says.

**Personality fit** is the one nobody audits honestly, and it also decides whether you're still here in five years. If reading someone else's code all day sounds miserable, software engineering stays exactly that. If ambiguity stresses you out, research stays ambiguous forever. Pick the day-to-day you can stand on a bad week, because the one that sounds best out loud is a different question entirely.

## where to go next

- [[getting-started]], for the overall roadmap and how to reverse engineer backward from whatever you picked here
- [[roadmap-by-year]], to see what your chosen track should look like at your current stage
- [[landing-your-first-internship]], for the search playbook once you have a direction
- [[building-experience-early]], if you're early and need experience before any of this applies

## turn this into action

Pick one track and one backup before you close this tab. Then find three entry-level postings in that track and read the requirements closely. The gap between those requirements and your current resume is your roadmap for the next year. The market wrote it, so you don't have to.

If nothing here felt like an obvious yes, pick anyway and default to software engineering. It's the widest door and the most transferable skill set, and every other track on this list is reachable from it later.
