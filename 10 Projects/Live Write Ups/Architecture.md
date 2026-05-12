# Architecture: Live Write Ups

## Data Schema (MDX)
Each writeup is stored as an `.mdx` file in `src/content/writeups/`.

```yaml
---
title: "SQLi on Google Search"
payout: "$10,000"
researcher: "HackerOne"
initial_step: "recon_start"
---
```

### Steps/Nodes
We will use a JSON-like structure within the MDX or a separate JSON file to define the graph:

```json
{
  "recon_start": {
    "text": "You start at the search bar. What is your first move?",
    "options": [
      { "label": "Search for special characters", "next": "fuzz_chars", "type": "correct" },
      { "label": "Look for subdomains", "next": "subdomain_recon", "type": "neutral" }
    ]
  },
  "fuzz_chars": {
    "text": "You see a 500 error when inputting `'`. Success! Now what?",
    "feedback": "Correct. Fuzzing parameters is the most direct way to find injection points.",
    "options": [...]
  }
}
```

## UI Components
- **DecisionCard:** Displays current step and choices.
- **FeedbackOverlay:** Shows explanation after a choice.
- **ProgressMap:** Visualizes the journey (optional).

## Tech Stack
- **Framework:** Astro JS
- **Styling:** Vanilla CSS / Tailwind (to be decided)
- **Content:** MDX
