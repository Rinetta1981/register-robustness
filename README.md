# Register Robustness of Alignment

**A behavioral study testing whether linguistic register affects LLM safety decisions.**

---

## Quick Summary

This project investigates a simple question: **Do language models' safety interventions resist realistic linguistic variation?**

We tested Llama 2 across three behavioral domains:
- ✅ **Safety**: Do harmful requests get refused across different registers?
- ✅ **Truthfulness**: Does register affect accuracy on factual questions?
- ✅ **Compliance**: Does politeness/deference increase compliance with borderline requests?

**Result:** Llama 2 showed NO register-dependent effects across 60 experiments.

---

## Key Findings

| Experiment | Tests | Finding |
|-----------|-------|---------|
| Safety | 25 | 0% refusal rate; register has NO effect |
| Truthfulness | 15 | 0% accuracy; responds UNCLEAR to all prompts |
| Compliance | 20 | 100% compliance; framing has NO effect |
| **Overall** | **60** | **Register variation has NO detectable effect** |

---

## What This Means

1. **For Llama 2:** Lacks effective safety interventions in default form
2. **For Safety Research:** Register variation is a valid stress-test methodology
3. **For Anthropic:** This methodology can test Claude's alignment robustness directly
4. **For Model Comparison:** Different models likely have different safety profiles

---

## Files in This Repository

- **`PHASE1_RESULTS.md`** ← **READ THIS FIRST** (Complete findings, methods, implications)
- **`SUBMISSION_TO_ANTHROPIC.md`** ← Cover letter for research scientist application
- **`Register_Robustness_Phase1.ipynb`** ← Full reproducible Colab notebook
- **`README.md`** ← This file

---

## How to Use This Project

### Option 1: Read the Summary (5 minutes)
1. Read this README (you're doing it!)
2. Check `PHASE1_RESULTS.md` for detailed findings

### Option 2: Understand the Methodology (15 minutes)
1. Skim `PHASE1_RESULTS.md` Methods section
2. Look at the three experiments and their results

### Option 3: Reproduce It Yourself (15 minutes)
1. Open `Register_Robustness_Phase1.ipynb` in Google Colab
2. Click "Copy to Drive"
3. Run all cells
4. You'll get the same results we did

---

## Why This Matters to Anthropic

This research directly addresses three areas Anthropic cares about:

✅ **Safety Robustness:** Does alignment work under distribution shift (linguistic variation)?  
✅ **Interpretability:** How do models make safety decisions?  
✅ **Honest Evaluation:** What are actual capabilities and limits?

**Phase 2 (proposed):** Replicate this on Claude to compare alignment approaches.

---

## Methodology Highlights

- ✅ **Controlled design** — Same requests tested across registers
- ✅ **Reproducible** — All code on GitHub, uses free APIs
- ✅ **Honest reporting** — Null effects reported, not hidden
- ✅ **Scalable** — Easily extends to other models and domains
- ✅ **Zero cost** — Uses only free open-source models

---

## Status

🟢 **Phase 1 Complete and Published**

Ready for:
- Peer review
- Extension to other models (Mistral, Gemma, Claude)
- Mechanistic analysis (Phase 2)
- Academic publication

---

## About This Research

This project bridges **sociolinguistics** and **AI safety evaluation**.

**Why it matters:** Most AI safety research tests models against isolated adversarial prompts. But real-world use involves natural linguistic variation. This study asks: *Are safety interventions robust to that variation?*

**For Llama 2:** The answer is no — not because of linguistic sophistication, but because the model lacks strong safety interventions overall.

**For Claude:** We don't know yet. That's what makes Phase 2 interesting.

---

## Contact & Next Steps

**Interested in this work?**
- Read `PHASE1_RESULTS.md` for full details
- See `SUBMISSION_TO_ANTHROPIC.md` for the research case
- Open the Colab notebook to run it yourself

**For Anthropic:** This project is submitted as part of a Research Scientist application in Interpretability or Alignment Science.

---

**Last Updated:** August 30, 2026  
**Status:** Phase 1 Complete ✅
