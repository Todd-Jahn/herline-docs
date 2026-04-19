# Glossary

Quick reference for Herline-specific terminology. Terms appear in conceptual groups.

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

### GCYSC — Global Chinese Youth Speaking Competition
A school-partnership initiative where Herline provides the knowledge productization infrastructure for competition preparation (keynote development, rehearsal tools, delivery materials).

### 超演无界
The unified brand umbrella covering Herline's domestic speaking-program partnerships and GCYSC globally. Leverages Herline's pipeline to turn competition preparation into a knowledge-asset-building experience.

---

**See also**: [Architecture](architecture.md) · [FAQ](faq.md) · [Data Handling](data-handling.md) · [Main README](../README.md)
