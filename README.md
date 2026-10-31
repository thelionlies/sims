# SIMS

A browser demo of the Social Impact Mapping Simulation — a vibecoded refactor of the [original Java project](https://github.com/thelionlies/SIMS-Social-Impact-Mapping-Simulation), made to run without a local Java setup.

**Live demo:** [thelionlies.github.io/sims](https://thelionlies.github.io/sims)

## What it simulates

Agents move around a shared space and try to persuade each other. Each agent belongs to a party (Red, Blue, or Undecided) and has a demographic profile (age group, sex). Opinions shift based on Social Impact Theory (Nowak, Szamrej & Latané, 1990).

Influence is weighted by:
- **Age similarity** — agents of the same age group influence each other more
- **Sex similarity** — agents of the same sex influence each other more
- **Distance** — closer agents have stronger influence (inversely proportional to distance²)

An undecided agent adopts whichever party has greater total influence on it. A committed agent switches only when opposing influence is stronger and at least one opposing neighbor is nearby.

## Controls

| Control | Description |
|---|---|
| Agents | Number of agents in the simulation |
| Speed | How fast agents move and how often opinions update |
| Age ↔ Sex influence | Balance between which demographic dimension drives influence |

## Original

Java implementation: [github.com/thelionlies/SIMS-Social-Impact-Mapping-Simulation](https://github.com/thelionlies/SIMS-Social-Impact-Mapping-Simulation)
