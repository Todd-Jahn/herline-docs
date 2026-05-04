# Glossary

Quick reference for Herline-specific terminology. Terms appear in conceptual groups.

## Brand Names

### Herline
The product name in English. Derived from "her" (for the female-led founding team and the predominantly female creator audience the product first served) + "line" (the vertical pipeline metaphor).

### 赫能 (Hè Néng)
The Chinese brand name. "赫" carries a sense of being conspicuously present in public; "能" means capability. The pair maps directly to the two-axis thesis — visible influence × built-up capability.

### 双核基础设施 (Dual-Core Infrastructure)
Internal positioning vocabulary for what Herline builds — "code + media" infrastructure on the company side, mirrored as "cognitive depth × public influence" capability on the user side. Roots in Naval Ravikant's wealth-leverage framework. See [Two-Axis Thesis](two-axis-thesis.md).

## Pipeline Layers

### Assessment
Onboarding layer that captures the user's professional profile — expertise domains, learning goals, communication preferences, target-audience profile. Drives personalization throughout the pipeline.

### Atlas
Recommendation / planning layer. Plans personalized book and content paths based on the user's Assessment profile. Conversational: users interact with Atlas as a knowledge planner.

### Library (D2B)
"Deep-to-Book." Deconstructs books into structured knowledge blocks (Claims / Concepts / Methods). Not summarization — structured extraction with citation traceability.

### Studio
Course strategy layer. Takes knowledge blocks (from the user's graph) and designs a course blueprint — units, learning arc, block-to-unit mapping, assessment approach.

### Courses (B2C)
"Book-to-Course." Generates full course content from a Studio blueprint — scripts, audio narration, assessments. Async-executed because generation can take 30–90 minutes for a full course.

### Prep
Delivery-format layer. Exports courses into presentable deliverables — PDF keynotes with timing, PPTX templates with speaker structure, DOCX teaching materials, quote cards.

### Boost
Multi-platform distribution layer. Adapts content for platform-specific formats (short-form video scripts, social posts, podcast adaptations, newsletter formats).

## Pipeline Agents

The pipeline is operated by named conversational agents, each scoped to one production phase. Users interact with them by name in the product UI.

### Helena
The main routing & dialog agent across Atlas (planning) and Library (deep-read). Handles intent detection, multi-turn conversation, and routing to specialized skills (D2B / RAG / recommendation). Most users meet Herline through Helena first.

### Holly
The course strategy agent operating in Studio. Takes a user's professional profile + selected knowledge blocks and proposes course briefs — positioning, audience, learning arc, unit structure. Holly hands off to the B2C generation engine once the brief is locked.

### Hera
The delivery-prep agent operating in Prep. Turns finished courses into stage-ready deliverables — keynote PDFs with timing notes, PPTX templates with structured talking points, DOCX teaching materials. Hera is the layer between "course exists" and "you can actually walk on stage with it".

### Hylia
The distribution agent operating in Boost. Adapts content for platform-specific formats — long-form social posts, short-form video scripts, podcast adaptations, newsletter framings. Hylia is what closes the public-influence loop on the two-axis thesis.

## Knowledge Unit Types

### Claim
A factual assertion extracted from source material, with citation to the originating passage. Example: *"System 1 thinking is fast and automatic (Kahneman, p. 24)."*

### Concept
A definable idea, framework, or entity. Example: *"Anchoring Effect"*, *"Peak-End Rule"*, *"Loss Aversion."*

### Method
A reproducible procedure, approach, or technique. Example: *"5-Why root cause analysis"*, *"Pre-mortem planning."*

### Knowledge Block
Umbrella term for a Claim, Concept, or Method. Each block includes source location, confidence signal, related-block links, and metadata for retrieval.

## Audience Terms

### Super Individual (超级个体)
Knowledge workers operating as one-person businesses, combining multiple roles (consultant, content creator, educator, coach) under a personal brand. Herline's primary user.

### One-Person Company (一人公司)
A business structure where a single person performs all roles — strategy, delivery, marketing, sales. Common in knowledge industries in China; over 12M practitioners by 2026.

### Knowledge Creator
Broader category including super individuals plus domain experts who produce educational content (teachers, trainers, writers) even if employed by institutions.

## Technical Terms

### Cross-Book RAG
Retrieval-Augmented Generation that spans the user's entire knowledge database, surfacing connections across books and readings. Enables course generation that composes insights from multiple sources.

### Knowledge Graph
The user's persistent, growing database of Claims, Concepts, and Methods extracted from all their deep reads. Grows with use; enables compounding productivity.

### Cross-Book Composition
The ability to build a single course or keynote from knowledge blocks drawn from multiple books — a capability that emerges from cross-book RAG plus the Studio layer.

### Pipeline Layer
One of the seven specialized stages (Assessment through Boost). Each layer has a typed input, typed output, and specific responsibility. Layers are usable standalone or chained.

### LangGraph Orchestration
The framework Herline uses to model each pipeline layer as a graph node (or subgraph) with explicit state transitions and checkpointing. Enables long-running jobs to resume from the last checkpoint rather than restarting.

### Async Generation
Long-running tasks (D2B extraction, B2C course generation, TTS synthesis) run on an async queue rather than blocking the UI. Jobs are observable via trace IDs and cancelable mid-execution.

## Product Tiers

### Free Tier
Entry-level access covering Assessment, a first deep-read, and a course generation trial. No credit card required.

### Core / Pro Tiers
Paid tiers with higher generation quotas, priority queues, and expanded storage. Details at [herline.vip/pricing](https://herline.vip) (linked, not reproduced here — see `feedback_marketing_page` convention).

### Institution Tier
For schools, training organizations, and institutions needing curriculum matrices and multi-teacher collaboration. Contact `partners@herline.vip`.

## Related Projects & IPs

### GCYSC — Global Chinese Youth Speaking Tour
An overseas-only school-partnership initiative where Herline provides the knowledge-productization infrastructure for partner schools running Chinese-language speaking programs — keynote development, rehearsal tools, delivery materials, cross-cohort archives. **Not connected to mainland-China admissions or credential systems.**

### 超演无界 (Chao Yan Wu Jie)
The unified brand umbrella covering Herline's speaking-program collaborations. The Chinese-domestic version operates under the "巡回" (tour) framing for educational compliance; the international version is GCYSC. Leverages Herline's pipeline to turn speaking-program preparation into knowledge-asset-building rather than ephemeral coaching.

---

**See also**: [Architecture](architecture.md) · [FAQ](faq.md) · [Data Handling](data-handling.md) · [Main README](../README.md)
