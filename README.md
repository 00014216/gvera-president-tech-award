# GVERA

**Lovable / Cursor for hardware.** GVERA is a vibe-building platform for non-technical people and hardware
teams: describe a device in plain words, or show a few reference pictures, and GVERA returns a finished,
buildable product.

Website: [gvera.app](https://gvera.app)

> This repository is a public overview for award and investor review. GVERA itself is proprietary
> software; its source code is not published here. See [LICENSE](LICENSE).

## The problem

Software got its "anyone can build it" moment with AI. Hardware did not. Turning an idea into a physical
product still takes CAD, electronics and firmware skills, expensive engineers and months of iteration,
and mistakes often only show up at assembly or testing. Most people with a hardware idea never build it,
and small teams spend their runway on prototypes.

## What GVERA does

```text
"build me a drone"  ──►  GVERA  ──►  3D CAD · circuit design · simulation · renders · launch page
```

- **Plain-language input.** Type what you want to build, optionally with up to five sample pictures
  ("a desk lamp like sample 1, in the black of sample 2").
- **AI agents that work like an engineering team.** GVERA breaks the request into requirements and a
  plan, then designs the mechanics, electronics and presentation of the product step by step.
- **Real engineering tools, not just text.** Designs are produced with established engines for CAD,
  circuit design (KiCad), physics simulation and rendering, so the output is real project files.
- **Every step is checked.** Each stage passes typed quality gates (for example electrical rule checks and
  simulation) before the next one starts, and the agents ask you when a decision is yours to make.
- **Resumable.** A project can be stopped at any moment and picks up exactly where it left off.

## Who it is for

- **Non-technical makers and founders** who have a product idea but no engineering team.
- **Hardware startups** that need to go from idea to prototype faster and cheaper.
- **Universities, robotics schools and labs** teaching engineering through real projects.

## Platforms

Desktop app for Windows, macOS and Linux, plus a terminal interface. AI requests run through GVERA Cloud
under the user's account.

## Status

- Working version in users' hands since October 2026; official launch upcoming.
- Paying users before launch, 350+ people in pilots and customer interviews.
- Partnership with Robotics Lab (robotics learning center); interest from education and agribusiness
  customers.
- UzCombinator alumni; "Excellence Award", SCO 5th Youth Innovation & Entrepreneurship Competition (2026).

## What is in this repository

| File | What it shows |
|---|---|
| [`schemas/requirements.v1.json`](schemas/requirements.v1.json) | How GVERA turns a plain-language request into numbered requirements, each with a priority and a verification method (analysis, simulation, test, inspection or demonstration). |
| [`schemas/netlist.schema.json`](schemas/netlist.schema.json) | The circuit format GVERA's electronics stage produces: components, pins and the nets that connect them, ready for circuit design and rule checks. |

## License

Copyright (c) 2026 GVERA Technologies. All rights reserved. Proprietary; see [LICENSE](LICENSE).
