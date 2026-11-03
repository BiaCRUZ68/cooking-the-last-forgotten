# The Last Forgotten Feast — Historical Cooking Video Workflow

> History isn't made only through wars and coronations — it's served at the table.

An instruction repository for turning researched historical food scripts into **physically readable, step-by-step culinary reconstructions**. Generate a detailed IMAGE prompt and a detailed VIDEO + AUDIO prompt for every shot, ready for tools such as VideoExpress/Express AI.

This is a production playbook, not executable cooking software, a video model, or a connected VideoExpress integration. It guides an AI agent; generated hand movements and food physics still require visual review.

## Start here

1. Load [SYSTEM_PROMPT.md](SYSTEM_PROMPT.md) into your agent, or ask it to read and follow that file.
2. Supply an episode script or script excerpt, a recipe/source if available, and your preferred cook visibility.
3. The agent maps recipe dependencies, locks the kitchen and cook, then writes paired prompts with synchronized culinary ASMR.
4. Generate and inspect each opening image before animating it. Transfer the accepted food state to the next shot.

```text
Follow SYSTEM_PROMPT.md.
Episode: [paste the approved English script]
Dish and sources: [paste recipe/evidence, or ask for research]
Scope: cooking chapter only
Cook visibility: hands-only
Setting: historically grounded reconstruction; establish period and place from the episode
Style: cinematic photorealistic cooking; antique watercolor-and-ink history inserts
Ratio: 16:9
Clip length: up to 10 seconds
Audio: off-screen narration and synchronized cooking ASMR; no dialogue or lip-sync
Return detailed IMAGE and VIDEO prompts in separate code blocks for every shot.
```

## What the workflow produces

- Evidence table separating DOCUMENTED, INFERENCE and RECONSTRUCTION decisions.
- Recipe quantities, preparation order, real process times, substitutions and unresolved gaps.
- Cook/kitchen continuity bible and explicit food-state ledger.
- Script-linked shots: narration, duration, purpose, opening state, action and ending state.
- Two self-contained prompts per shot, including hand/tool choreography and material behavior.
- Sound plan, timeline assembly notes and targeted QA.

For a request covering only one script excerpt, output only its necessary shots and short relevant continuity notes.

## Modes

| Choice | Options |
|---|---|
| Cook visibility | Hands-only; full-cook; hybrid |
| Kitchen | Period reenactment; explicitly modern historical test kitchen |
| Cooking visuals | Cinematic photorealism (default); antique watercolor and ink |
| Historical inserts | Antique watercolor and ink (default); user-selected treatment |
| Production | Prompt package (default); asset generation/assembly only when requested and available |

A hands-only cook still has a fixed Actor 1 identity, sleeves and hands. Full-cook shots use the same reference, wardrobe and kitchen. No compulsory speaking presenter. Long episodes are supported; clips remain at most 10 seconds unless the user specifies another supported limit. There is no inherited five-minute episode cap.

## Files

- [SYSTEM_PROMPT.md](SYSTEM_PROMPT.md): complete agent instructions.
- [docs/SOURCE_ANALYSIS.md](docs/SOURCE_ANALYSIS.md): analysis of the reference and adaptation decisions.
- [docs/ACTION_LIBRARY.md](docs/ACTION_LIBRARY.md): egg cracking, whipping, folding, slicing, kneading, pastry and heat actions.
- [docs/QA_CHECKLIST.md](docs/QA_CHECKLIST.md): checks before and after generation.
- [templates/EPISODE_BRIEF.md](templates/EPISODE_BRIEF.md): reusable production brief.
- [templates/SHOT_TEMPLATE.md](templates/SHOT_TEMPLATE.md): paired-prompt output format.
- [templates/STATE_LEDGER.json](templates/STATE_LEDGER.json): reusable tracking structure.
- [examples/EGG_WHITE_TECHNIQUE.md](examples/EGG_WHITE_TECHNIQUE.md): complete modern demonstration of separate preparation, whipping, endpoint and folding shots.

## Boundaries

Research is required before historical claims are added. Generated footage illustrates a reconstruction; it is not evidence that a method occurred. Modern test quantities must not be presented as surviving historical measurements. Unsafe historical foods are discussed or simulated, not recreated for consumption.

Repository: https://github.com/BiaCRUZ68/cooking-the-last-forgotten

Open SYSTEM_PROMPT.md to start. This repository contains the workflow, templates and examples; using it requires an AI agent with the appropriate research or generation tools.
