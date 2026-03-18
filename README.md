# 🎬 ConceptDrop

**Drop a concept. Get a scroll-stopping animation.**

A Claude skill that turns any mental model, framework, or idea into a polished 5-7 second animated explainer — ready to screen-record and post to LinkedIn, Twitter, or use in presentations.

No design tools. No video editors. No prompting gymnastics. Just say the concept.

---

## How It Works

```
You:    "80/20 rule"
Claude: → Generates a full animated React artifact
You:    Screen-record → Post to LinkedIn
```

**That's it.** Claude automatically:
- Finds the core tension ("most people think X, but actually Y")
- Picks the best visual scheme (from 10 animation patterns)
- Writes a scroll-stopping hook + punchline
- Generates a production-ready animated artifact

### For niche or unfamiliar concepts
If Claude doesn't fully understand the concept, it asks 2-3 quick clarifying questions first — then generates. This means you can animate your own proprietary frameworks too, not just well-known mental models.

---

## Examples

| Input | Hook | Visual | Punchline |
|-------|------|--------|-----------|
| `80/20 rule` | "Where do results REALLY come from?" | Grid highlight + bar chart | "Stop doing more. Start doing what matters." |
| `sunk cost fallacy` | "Why do you finish BAD MOVIES?" | Stacked costs ✕ crossed out → decision card | "What you've spent is gone. Only what's ahead matters." |
| `compound interest` | "Why do the rich keep getting richer?" | Counter morph showing exponential growth | "Time in the game beats timing the game." |
| `dunning-kruger` | "When do you THINK you know the most?" | Gauge that spikes early then dips | "The peak of confidence is the valley of competence." |

---

## Animation Spec

| Property | Value |
|----------|-------|
| Format | React (.jsx) artifact |
| Dimensions | 540 × 540px (1:1 square) |
| Duration | ~8 seconds |
| Background | Dark (#0a0a0a) |
| Typography | System sans-serif |
| Colors | Single vibrant accent + white/gray |
| Animation | CSS keyframes only, no external libs |
| Watermark | Customizable (bottom-left) |

### The Narrative Arc

Every animation follows this structure:

```
PROVOCATIVE QUESTION → STATE A → TRANSFORMATION → STATE B → PUNCHLINE
```

| Phase | Timing | What Happens |
|-------|--------|-------------|
| Title | 0.0s – 0.8s | Hook question fades in |
| State A | 0.8s – 2.5s | "Before" visual animates in |
| Transform | 2.5s – 3.8s | The shift / reveal moment |
| State B | 3.8s – 5.2s | "After" visual animates in |
| Punchline | 5.2s – 6.8s | Bold takeaway slides up |
| Hold | 6.8s – 8.0s | Everything visible for reading |

---

## 10 Visual Schemes

Claude auto-selects the best one based on your concept:

| # | Scheme | Best For | Example Concept |
|---|--------|----------|----------------|
| 1 | Pie Chart Shift | Time/effort redistribution | "AI replacing PM work" |
| 2 | Bar Chart | Magnitude comparisons | "80/20 rule" |
| 3 | Scale/Balance | Trade-offs | "Work smarter not harder" |
| 4 | Funnel | Filtering, narrowing | "Why startups fail" |
| 5 | Stacked Blocks | Composition shifts | "Technical debt" |
| 6 | Counter/Morph | Surprising statistics | "Compound interest" |
| 7 | Path/Timeline | Evolution, progression | "Career stages" |
| 8 | Venn Shift | Overlap changes | "Product-market fit" |
| 9 | Gauge/Meter | Thresholds, tipping points | "Burnout" |
| 10 | Grid/Highlight | Vital few vs trivial many | "Signal vs noise" |

---

## Usage

### Quick Start
```
animate: survivorship bias
```

### With Context
```
concept video: network effects — for startup founders
```

### With a Preferred Visual
```
use a funnel for the hiring pipeline concept
```

### For Your Own Frameworks
```
animate: our CA trust proxy model
```
_(Claude will ask clarifying questions first, then generate)_

---

## How to Record & Post

1. Open the artifact full-screen in Claude
2. Hit **↻ Replay**
3. Screen-record (~8 seconds)
   - **iPhone**: Swipe down from top-right → Screen Recording
   - **Mac**: `Cmd + Shift + 5` → Record Selected Portion
   - **Windows**: `Win + G` → Game Bar
4. Trim to the animation → Post to LinkedIn as video

---

## Installation

Download the `concept-animator.skill` file and add it to your Claude skills.

---

## Customization

To change the watermark, edit this line in `SKILL.md`:

```jsx
serin paul  →  your name here
```

---

Built with Claude. Animated with CSS. Posted with confidence.
