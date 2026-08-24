# Energy → Compute Flow Terminal

A Bloomberg-terminal-style map of the venture landscape between primary energy and AI compute, built around the thesis that the AI buildout is a continuous physical process that turns electrons into tokens and heat. Every company sits somewhere on that flow. In a lossy flow with moving bottlenecks, the interesting opportunities either shorten the flow, by removing losses, steps, or waiting, or own a point it cannot route around, positions made of physics, law, or institutional process. And the two moves run as a sequence: shorten to enter, own to stay.

The terminal maps 456 companies across the US, Canada, Europe, and beyond, along the electron's journey: 01 Siting, Permits & Financing · 02 Generation & Site Power · 03 Grid Interconnect & Transmission · 04 Facility Power Conversion (800VDC) · 05 Rack & Board Power · 06 Transient Load Management · 07 Compute & Memory · 08 Interconnect & Networking · 09 Thermal Management · 10 Physical Execution · 11 Compute Provisioning & Orchestration.

## Why this exists

Market maps in this space get rebuilt every time the binding constraint shifts, grid headroom one year, turbine order books the next, then transformers, electricians, water permits. The physical process never gets rebuilt: electrons must be generated, transmitted, converted, computed with, and their heat rejected, in that order, every time. Organizing the landscape by the electron's journey instead of by market category gives a taxonomy that doesn't go stale, and it matches how founders in this space actually describe what they do, which is what makes it useful as a working instrument rather than a survey.

## Using it

❖ THESIS — the full essay behind the map, *The Electrons Must Flow*: what the buildout is physically, the two moves, where founders are actually showing up, and a walk down the flow in eight stops. Company names in the essay open their live dossiers in the terminal, stage chips jump into the flow, and a typeset PDF is one click away.

◈ FLOW — click any stage for a full brief: what the stage is, key numbers, why it binds now, how the work is done today, pain points, the two moves at this stage (shorten / own / timing, written from the thesis), open seats, analyst reading, news, and every company mapped to it. The open seats are derived methodically: each stage's physics defines its constraints, the company map shows where solutions cluster, and a gap is an empty seat inside proven crowding, stated with its cluster evidence and entry signal.

☰ COMPANIES — the full table. Multi-select filters (combine stages, rounds, geographies: US / Canada / Europe / Intl), founded-year range, free-text search across names, descriptions, and investors. Star companies to build a watchlist (persists in your browser), filter to saved, export any view as CSV.

✦ NEWS — 150+ dated items grouped by month, filterable by stage, every one linked to its source; the primary sources cited in the thesis, from the IEA and LBNL to Duke's *Rethinking Load Growth* and the memory-wall literature; and an analyst commentary, essays, and institutional reports layer spanning SemiAnalysis, Ribbit Capital, Construction Physics, Nutty, Citrini Research, Irrational Analysis, Doomberg, Epoch AI, MIT Technology Review, EPRI, Grid Strategies, CB Insights, Currence, and others.

◈ QUERY TERMINAL (bottom right) — a chat interface over the data. It runs entirely in your browser: a deterministic query engine over the embedded dataset, no AI model, no API calls, no account, no cost. It remembers context, so you can refine: canadian companies → of those, only seed → save all. Try brief stage 9, largest raises at stage 2, nuclear startups founded after 2023, or type help.

## How it was built

Built in Claude (Anthropic's Cowork mode), with research and engineering in the same working sessions. The research layer combined the Exa deep-research connector, parallel research agents across several thousand sources, and a Specter talent-graph pass for discovery and enrichment, with every candidate verified against live sources; unverifiable names were dropped rather than kept. The artifact is deliberately boring technology: a single self-contained HTML file, vanilla JavaScript, embedded data, no framework, no build step, no backend, no dependencies. It runs from a double-click and deploys as a static file.

## Approach and sources

Three rules govern the data. Primary sources over aggregators: numbers are anchored to the analyst or filing that produced them. Dual-sourcing and dated verification: every company entry carries a last-verified date, and thinly-sourced claims are flagged in the entry itself. Asymmetric depth: coverage is deepest on the energy-heavy stages where the thesis concentrates, and honest about being lighter on compute silicon and networking, where others have deeper conviction.

## Data notes

The dataset is a point-in-time snapshot, refreshed regularly; every company entry carries its own last-verified date. Companies confirmed inactive are removed on discovery; acquired-but-operating companies carry a status note. Watchlists are stored locally in your browser, nothing leaves your machine, and the only external request the page makes is for fonts.

## Running locally

Download index.html and open it in any browser. Fully self-contained: no server, no build step, no network required. The thesis is also available as a standalone PDF, `the-electrons-must-flow.pdf`.

## What's next

Deeper enrichment (entry valuations and headcount growth per company, so the map can weigh opportunities, not just locate them), a shorten/own tag on every company so the thesis becomes a filter, capacity- and dollar-weighted stage views alongside company counts, continued geographic expansion, and regular refresh cycles feeding the news and company layers.

Corrections and additions welcome via issues. The map improves when it's argued with.

Nothing here is investment advice.
