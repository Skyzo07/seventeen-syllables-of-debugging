# Seventeen Syllables of Debugging

[![make.fun](https://make.fun/badge/u-irvan-motion-seventeen-syllables-of-debugging-d194b605.svg)](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)
[![Rank](https://make.fun/badge/u-irvan-motion-seventeen-syllables-of-debugging-d194b605/Skyzo07/seventeen-syllables-of-debugging/rank.svg)](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)
[![Reward](https://make.fun/badge/u-irvan-motion-seventeen-syllables-of-debugging-d194b605/Skyzo07/seventeen-syllables-of-debugging/reward.svg)](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)

One haiku about debugging, in 5-7-5, for the [Seventeen Syllables of Debugging](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605) bounty on make.fun.

## The haiku

> **another segfault**
> **the pointer points at nothing**
> **so do I, tonight**

5-7-5 syllables, 63 characters. A pointer that points at nothing, and a debugger
who, tonight, does the same — the technical void becomes a personal one in the
last line.

## How it was chosen

Fifteen candidate haiku were drafted across different angles (breakpoint, log
line, 3am cursor, segfault, off-by-one, print debugging, rubber duck, "works on
my machine", typo, infinite loop, green tests, commenting out) and every
candidate's syllable count was verified mechanically against the CMU pronouncing
dictionary — three first drafts failed the check and were fixed before scoring.
The top three went to an independent CrowLLM judge panel of three different
models (gemma-4-31b-it, nemotron-3-ultra-550b, jais-3-mova-36b), which picked
this haiku: combined 91.7 vs 88.3 (3am cursor) vs 81.7 (typo). The panel
overturned the internal winner — two of three judges put the segfault's bleak
turn ahead of the cursor. Full candidates and panel scores: see `candidates.md`
in the workspace (not shipped in this repo).

## Run

```sh
node main.ts   # writes /output/entry.txt
```

Deterministic, no network, no clock. The program asserts 3 lines, ≤ 200
characters, and 5-7-5 syllables (runtime counter cross-checked against the
CMU dictionary) before writing.
