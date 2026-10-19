# Hole Rescue Workshop

Planning package for a single-screen YouTube Playables rescue puzzle, published through the MediaCube route.

The player moves a hole, eats debris to grow, keeps useful tools, builds a safe route and rescues one animal.

## Read first

- [AI build, platform, revenue and acceptance contract](hole-rescue-workshop-ai-build-contract.txt) — authoritative full specification, version 1.5.
- [Repository instructions](AGENTS.md) — implementation handoff and scope safeguards.
- [Concept gameplay mockup](docs/concept-gameplay-mockup.png) — sequence reference only; it does not prescribe graphics and is not a runtime asset.

## Accepted scope

| Item | Requirement |
| --- | --- |
| Puzzle bank | 3,000 genuinely distinct, validated levels, including the teaching sequence |
| Screen | Entire active puzzle and essential controls visible together |
| Rescue | One animal per level; free Undo, Reset and Replay |
| ZIP budget | At most 750,000 bytes for the complete runtime release |
| Expanded runtime | Below 999,000 bytes |
| Initial game-owned compressed transfer | At most 500,000 bytes |
| Pre-roll | YouTube-managed during initial loading |
| Interstitial | After two qualifying rescues AND 90 active gameplay seconds, at an informed Next/Replay transition after the payoff |
| Rewarded | One completed video earns one detailed next-action hint |
| Reward protection | Suppress interstitials for the rest of that attempt and at least 90 further active seconds |
| Final level | Preserve 3,000/3,000 progress and offer free same-screen Mastery replay; no interstitial on initial entry |

Mastery shuffles the 2,996 verified non-teaching puzzles without repetition within a cycle. Repeated puzzles remain clearly identified as replay. Bank first-clear progress never resets.

The earlier proposal of 12 animal types in four functional families is retained for implementation review. Exact behavioral bounds remain unresolved; animal skins do not increase the count of distinct puzzles. The full contract records the proposed species and the required validation.

## Build handoff

1. Read the contract and repository instructions.
2. Build one complete rescue, save/reload and Next/Replay flow; measure input and package size.
3. Resolve mechanical-depth and animal-profile rules with concrete evidence.
4. Validate genuinely different content at 100, 1,000 and 3,000 accepted entries. Keep offline generators, solvers and QA outside the runtime ZIP.
5. Implement the accepted host integration, ads and Mastery behavior under the contract; validate the exact release bytes.

Graphics remain unspecified. The mockup illustrates the loop and does not establish final art, layout dimensions, audio controls or asset requirements.

## Evidence status

This upload contains planning documents and a concept image. No game implementation, 3,000-level bank, measured runtime ZIP, executable game test result, device/host certification or platform publication is delivered here. The size limits are budgets, and the ad cadence is an accepted starting configuration, not a measured revenue optimum.

The contract contains the platform sources, pinned Haircut integration reference, limited mathematical-model results and full acceptance matrix. Preserve its distinction between approved choices, proposals and actual evidence.

Prepared and accepted for repository upload on 18 October 2026, America/Toronto.
