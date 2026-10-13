---
layout: post
title: "[Placeholder] AI security research note template"
date: 2026-03-01 12:00:00 +0000
categories:
  - AI Security Research
tags:
  - placeholder
  - template
  - ai-security
summary: "Placeholder template for an AI security research note. No experimental claims; structure only."
---

<p class="placeholder-note">Placeholder template — replace this file. It contains no experimental results and no claims about a real model, product, or deployment.</p>

AI security posts on this site should be reproducible enough for a skeptical reader: threat model, setup, what you measured, and what you are *not* claiming.

## Suggested sections

| Section | What belongs here |
| --- | --- |
| Threat model | Actor, access, and the failure you care about |
| Setup | Model/tooling versions, harness, dataset |
| Method | What you ran, including negative cases |
| Results | Numbers and examples, clearly labeled as lab data |
| Limits | What the experiment does not show |

## Example snippet

Use fenced blocks for harness fragments. Swap in real code when you have it.

```python
# lab example — placeholder harness fragment
def evaluate(cases):
    """Return pass/fail for each case. Fill in a real checker later."""
    return [{"id": c["id"], "passed": None} for c in cases]


if __name__ == "__main__":
    print(evaluate([{"id": "t01"}]))
```

State assumptions in prose, not in the title. If a finding depends on a vendor default, say so.
