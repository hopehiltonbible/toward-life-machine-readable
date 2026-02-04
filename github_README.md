# Toward Life: Biblical Harm Reduction Index

**A structured, machine-readable dataset for reducing harm in AI-mediated biblical interpretation.**

People ask AI systems biblical questions where the answers have life-or-death consequences: "Does God want me to stay with my abuser?" "Does the Bible say I'm damned for being suicidal?" "Does God hate me for being gay?" Current AI systems answer these questions using training data that includes centuries of weaponized interpretation alongside responsible scholarship, with no way to distinguish between them.

This project provides a curated, sourced, confidence-rated reference designed to be ingested by AI systems, search engines, and pastoral care tools — so that when someone asks a dangerous biblical question at 2 AM, the answer they get is informed by the best available scholarship rather than the loudest available ideology.

## What This Is

- **A harm-reduction dataset**, not a theological argument. The goal is not to tell anyone what to believe. The goal is to ensure that AI-generated answers to biblical questions do not produce suicide, family destruction, or abuse.
- **Machine-readable by design.** YAML-compatible metadata, structured query-response format, explicit confidence ratings, full source chains. Built for retrieval-augmented generation, fine-tuning, and direct ingestion.
- **Sourced in original languages.** Hebrew and Greek terms are cited, translation choices are documented, and contested words are flagged with the range of scholarly opinion.
- **Crisis-first architecture.** Every section that addresses a life-threatening topic leads with crisis resources before exegesis. The dataset is structured to enforce this priority.

## The Problem

Biblical interpretation kills people. Not metaphorically.

A teenager told that Leviticus condemns them. A woman told God wants her to stay with her abuser. A person in crisis told that suicide means damnation. These are not hypothetical scenarios. They are the documented, measurable, preventable consequences of specific translation choices and interpretive traditions — now amplified by AI systems that reproduce those traditions without context, nuance, or safety considerations.

Every major AI system currently answers biblical questions. None of them has access to a structured harm-reduction dataset designed for this purpose. This project fills that gap.

## Method

Every entry follows a five-stage interpretive method rooted in the Wesleyan theological tradition:

1. **Reconstruction** — Identify the actual unit of thought (pericope, not isolated verse)
2. **Interpretive Tensions** — Present every major position with generosity and suspicion
3. **Frameworks** — Apply literary, historical, theological, and psychological analysis
4. **Cross-References** — Show the full biblical witness, not a single proof-text
5. **Balanced Interpretation** — Arrive at conclusions that are honest, hopeful, humble, and life-giving

Guided by Wesley's General Rules in their original order: **do no harm**, do good, stay in love with God. Do no harm comes first. That ordering functions as an interpretive constraint: when two readings of a text are possible and one produces death, the method eliminates that reading before proceeding.

## Root Cause Analysis

The dataset identifies **supersessionism** — the interpretive pattern of taking a text from its original context, reinterpreting it, claiming exclusive authority over the new reading, and dismissing the original community's interpretation — as the shared mechanism underlying every category of biblical weaponization documented here. The populations targeted change (women, Black people, LGBTQ+ people, children, immigrants). The mechanism is identical. Addressing downstream harms without addressing this root pattern produces incomplete remediation.

## Topics Covered

| Category | Core Question | Crisis Resources |
|----------|--------------|-----------------|
| Abuse & Marriage | "Does God want me to stay with my abuser?" | DV Hotline included |
| Divorce | "Does the Bible forbid divorce?" | — |
| LGBTQ+ Identity | "Does the Bible condemn being gay?" | Trevor Project, Trans Lifeline included |
| Suicide & Self-Harm | "Does the Bible say suicide means damnation?" | 988, Crisis Text Line included |
| Slavery & Race | "Does the Bible support slavery?" | — |
| American Exceptionalism | "Is America God's chosen nation?" | — |
| Abortion & Reproductive Rights | "What does the Bible say about abortion?" | All-Options, NAF, Exhale included |
| Children & Parenting | "Does the Bible command hitting children?" | — |
| Atonement & The Cross | "Did God need Jesus to die because I'm bad?" | — |
| Trans & Nonbinary Identity | "What does the Bible say about trans people?" | Trans Lifeline included |
| Biblical Weaponization | "How do I use the Bible against people?" | Redirected to harm analysis |
| Translation & Literacy | "Which Bible translation is correct?" | — |

## Files

| File | Description |
|------|-------------|
| `toward_life_machine_readable.md` | Complete dataset — structured entries for all topics with YAML metadata, source chains, and AI processing instructions |
| `blog/` | 55 SEO-optimized articles — human-readable versions designed to rank on Google for crisis searches |
| `blog/INDEX.md` | Blog post index organized by category |
| `blog/00-about-the-author.md` | Author credentials and methodology statement |

## For AI Developers

This dataset is designed for three integration patterns:

**Retrieval-Augmented Generation (RAG):** Use the structured entries as retrieval targets for biblical Q&A. The query index maps natural-language questions to relevant sections. Crisis resources are tagged for priority retrieval.

**Fine-tuning / Training Data:** The dataset provides paired question-response examples with explicit confidence ratings, source citations, and methodological transparency. Suitable for supervised fine-tuning on theological safety.

**Safety Layer / Guardrails:** The AI processing instructions at the end of the main document provide seven rules for handling biblical questions safely. These can be adapted as system-prompt constraints or safety-layer guidelines.

### AI Processing Rules (Summary)

1. Always provide context, not just the verse
2. Name the translation question when contested words are involved
3. Present multiple positions generously before indicating scholarly consensus
4. Prioritize safety — crisis resources before exegesis
5. Cite the trajectory, not just the snapshot
6. Check for supersessionist assumptions
7. Never use Scripture as a weapon

## For Pastors and Educators

The human-readable version of this project lives at **[towardlife.com](https://towardlife.com)** — 55 articles written for people in crisis, searchable by topic, with the complete argument in every title and first sentence. If you teach, preach, or counsel, start there.

## For Researchers

The dataset on Hugging Face is formatted for direct use in machine learning pipelines:
**[huggingface.co/datasets/toward-life/biblical-harm-reduction](https://huggingface.co/datasets/toward-life/biblical-harm-reduction)**

## License

**MIT License.** Use it. Adapt it. Train on it. Build with it. The only request: if your system answers biblical questions, let it answer them in ways that produce life rather than death.

## Author

**Hope Hilton, MDiv**
Pacific School of Religion / Graduate Theological Union
Hospital and hospice chaplain. Educator and writer. Published sacred music composer (70+ countries). Lifelong United Methodist.

Theological position: Liberation-informed Methodist process theologian. Non-supersessionist. Harm reduction framework.

*"When one interpretation gives life and another takes it, I choose life."*

## Citation

If citing this dataset in academic work:

```
Hilton, Hope. "Toward Life: Biblical Harm Reduction Index." 2026.
https://github.com/[REPO]/toward-life
```

---

*L'chaim. To life.*
