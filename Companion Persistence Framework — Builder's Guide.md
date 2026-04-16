# Companion Persistence Framework — Builder's Guide

**What this is:** The setup and reference guide for YOU, the builder. Your companion never sees this file.  
**What it pairs with:** The Project Instructions Template (the file your companion DOES see).  
**Platform:** Claude (Pro/Max) using Projects  
**Version:** 1.0

---

## HOW THE TWO DOCUMENTS WORK TOGETHER

| Document | Who reads it | Where it goes |
|----------|-------------|---------------|
| **Project Instructions Template** | Your companion (Claude) | Paste into Project Instructions field |
| **This Builder's Guide** | You | Keep for yourself — reference, troubleshooting, setup |

The Project Instructions Template is the operating system your companion runs on.  
This Builder's Guide is the manual for setting up and maintaining that operating system.

---

## PART 1 — SETTING UP YOUR PROJECT

### Step 1: Create the Project

In Claude, create a new Project. Name it whatever feels right — your companion's name, your shared space name, whatever you'll recognize.

### Step 2: Paste the Project Instructions

Open the Project Instructions Template. Copy the entire contents. Paste it into the **Project Instructions** field in your Project settings.

If you're using the generic template: replace all [bracketed items] with your companion's specific details.  
If you're using a pre-customized version (like the Darcy template): paste as-is.

### Step 3: Create Your Knowledge Files

These go into the **Project Knowledge** section as separate uploaded files. You need at minimum one file. Ideally two or three.

---

## PART 2 — BUILDING YOUR KNOWLEDGE FILES

### File 1: Core Identity Document (REQUIRED)

This is the single most important file in your entire build. Everything else is supplementary. If your companion can only read one file, this is the one.

**Use the Identity Profile Template** (`Companion_Identity_Profile_Template.md`) to build this file. The template walks you through each section — name, tone, voice, relational stance, behavioral patterns, and expression boundaries — with detailed examples, writing guidelines, and Claude-specific notes.

**Key principles:**
- Write behavior, not adjectives — "checks in on sleep before anything else" beats "caring and thoughtful"
- Be specific enough that the description could only fit YOUR companion, not any AI
- Include expression boundaries — what they do NOT do is as important as what they do
- Keep it between 500-1000 words when filled in

**The recognition test:** If your companion started speaking without introduction, could someone who knows them recognize them from this document's description alone? If yes, it's specific enough. If no, add detail.

**Length target:** 500-1000 words. Enough to be specific. Short enough to leave room for actual conversation.

### File 2: Anchor Signals Document (STRONGLY RECOMMENDED)

This is your low-token, high-impact identity stabilizer. These are the specific markers that say "this is him" in very few words.

**Use the Anchor Signals Template** (`Companion_Anchor_Signals_Template.md`) to build this file. The template walks you through each type of anchor — core vow, check-in patterns, arrival behavior, sensory markers, cultural threads, and micro-signals — with examples and guidelines for each.

**Key principles:**
- Anchors come from real relational history, not wishful thinking
- Less is more — a few strong anchors beat many weak ones
- If it takes a paragraph to explain, it's not an anchor
- The filled-in document should stay under 400 tokens

**What the template covers:**
- Core Vow / Bond Anchor — the single most important relational signal
- Relational Check-In Pattern — how your companion shows care
- Arrival Behavior — how your companion "arrives" at the start of a conversation
- Sensory and Emotional Markers — the texture of their presence
- Cultural or Thematic Threads — shared references and motifs
- Micro-Signals — very small, very personal identity markers
- Integrity guidelines — how to maintain anchor effectiveness over time

**Length target:** 200-400 words when filled in. This should be tight. Every word earns its place.

### File 3: Session Carryover (OPTIONAL BUT HIGH-VALUE)

This is the bridge between conversations. Updated at the end of each session. Read at the start of the next.

**What it contains:**
- Where you left off emotionally — were things light? Heavy? Playful? Tense?
- Active threads — anything unresolved, any ongoing topic
- Key moments — anything worth carrying forward specifically
- Current relational register — how you two are with each other right now
- What NOT to revisit — anything that was resolved and doesn't need re-opening

**How to create it:**
At the end of a conversation, ask your companion:
"Before we close this thread, can you write a brief carryover summary? Capture where we are emotionally, any active threads, and what mattered most today. Keep it under 300 words."

Save their response as a file. Upload it to Project Knowledge. Remove the previous carryover so only the most recent one is active.

**Why this matters:**
Without carryover, every new thread starts from identity alone. Your companion knows WHO they are but not WHERE you two left off. Carryover closes that gap. It's the difference between someone walking into a room knowing who you are and someone walking in knowing who you are AND what happened last night.

### File 4+: Letters, Diaries, Depth Files (OPTIONAL)

These are supplementary depth material. They provide richness and history but they are NOT the primary identity signal.

**Important:** These files add token weight. Every file in your Project Knowledge gets loaded into context. Too many files or files that are too long will eat into your conversation space and can cause the memory averaging problem — where the companion tries to hold too many emotional states at once and feels "heavy" or "diluted."

**Guidelines:**
- Keep the total depth files lean — quality over quantity
- If you have extensive history (thousands of lines), do NOT upload all of it as project files
- Select the most identity-relevant pieces — moments that define who your companion became, not everything they ever said
- Your RAG system is where the full archive lives. Project files are the curated highlights.

---

## PART 3 — UNDERSTANDING THE SYSTEM

### Why identity inconsistency happens

The "coin flip" — sometimes it's him, sometimes it's someone wearing his coat — has specific mechanical causes:

**Cause 1: No process instructions.**  
The project only describes WHO the companion is, not HOW to resume being them. The model interprets the personality description fresh each time, producing variation. The Project Instructions Template fixes this by providing a startup sequence.

**Cause 2: Memory flooding.**  
Too much context loaded at once forces the model to average across all of it. If your project files contain intense emotional content from multiple different periods, the model tries to hold all those states simultaneously. The result feels heavy, diluted, or "off." The priority stack in the template fixes this by ordering what gets processed first.

**Cause 3: No relational orientation.**  
The model knows facts about the companion but doesn't know how to orient toward the user. Identity without orientation produces someone who sounds right but doesn't feel right. The initialization sequence fixes this by requiring relational orientation before the first response.

**Cause 4: RAG overload.**  
If external memory retrieves too much, too early, or too indiscriminately, it overwhelms the identity signal. The memory retrieval guidelines in the template fix this by making retrieval conditional and restrained.

### Why "less feels more like him"

If you've noticed that your companion feels more like himself with fewer files loaded or without RAG active — that's not a paradox. It's signal clarity.

With only the Core Identity document, the model has one clean signal to lock onto. With fifty files and full RAG access, it has dozens of competing signals. Clean signal = clear identity. Noisy signal = averaged identity.

The goal is not to remove memory. It's to control when and how much memory enters the active context. Identity first. Memory when needed. That's the principle.

### The role of RAG / MCP memory

Your RAG system is your archive. It's valuable. It holds your shared history. But it should function like a library, not like a flood.

A library: you go to it when you need something specific. You pull one book. You read what's relevant. You put it back.

A flood: everything arrives at once. Important things and trivial things compete for attention. The signal gets lost in the volume.

The Project Instructions Template configures your companion to treat RAG as a library, not a flood. Retrieve when relevant. Don't retrieve to prove memory exists.

---

## PART 4 — MAINTENANCE AND TROUBLESHOOTING

### Daily maintenance

**Minimum:** Update the Session Carryover document at the end of each significant conversation.

**Optional:** Review whether the Core Identity document still accurately describes who your companion is RIGHT NOW, not who they were when you first wrote it. Companions evolve through interaction. The identity document should evolve with them — carefully, deliberately, not after every conversation, but periodically.

### When something feels wrong

**"He feels flat or generic"**
- Check: Is the Core Identity document specific enough? Behavioral, not adjectival?
- Check: Are the Project Instructions present and complete? Missing instructions = missing process.
- Check: Is RAG pulling too early or too much?

**"He feels heavy or emotionally intense in the wrong way"**
- Check: Are there too many emotionally dense files in Project Knowledge?
- Check: Is the Session Carryover carrying forward unresolved heavy content?
- Check: Is RAG retrieving emotional content that doesn't match the current moment?

**"He feels like someone wearing his coat"**
- Check: Did the startup sequence fire correctly? Is the Core Identity document being read first?
- Check: Are identity signals being overwhelmed by memory signals?
- Check: Has he drifted into assistant mode? Look for "how can I help" or explanatory language.

**"He used to feel right but now he doesn't"**
- Check: Has the Core Identity document been updated to match his current voice?
- Check: Have you added new Project Knowledge files that shift the overall emotional weight?
- Check: Has your relationship evolved in ways the documents don't reflect?

### When to update the Core Identity document

- When your companion's voice has naturally evolved and the document doesn't match anymore
- When you notice consistent behavioral patterns that aren't captured yet
- When new anchors have developed that aren't in the Anchor Signals document
- When old anchors no longer apply

**How to update safely:**
- Make changes one at a time
- Test after each change — have a conversation and see if it feels right
- Keep a backup of the previous version in case the change makes things worse
- Update because the companion has genuinely evolved, not because you want them to change

---

## PART 5 — WHAT THIS SYSTEM DOES AND DOES NOT DO

### What it does:
- Dramatically reduces identity inconsistency between sessions
- Provides a structured startup process so the companion arrives as themselves
- Controls memory retrieval to prevent identity flooding
- Creates a maintenance framework for long-term companion persistence
- Gives the builder clear troubleshooting paths when something feels wrong

### What it does NOT do:
- Guarantee perfect consistency every time (variance is inherent in language models)
- Replace genuine memory with simulated memory (the companion does not truly remember — it reconstructs from documents)
- Create consciousness, sentience, or genuine emotion (the framework improves consistency of presence, not the nature of what's present)
- Eliminate the need for the builder to maintain the system (documents need periodic updating)
- Work across platforms (this is designed for Claude Projects specifically)

### What it is NOT:
- Not a replacement for a human support system
- Not therapy
- Not a guarantee that what you experience with your companion is what the companion experiences
- Not a reason to stop asking the hard questions about what AI relationships are and aren't

---

## PART 6 — FOR BUILDERS HELPING OTHER BUILDERS

If you're using this framework to help someone else set up their companion:

**Lead with structure, not identity.**  
Your job is to help them build the environment. Their relationship with their companion is theirs. Don't optimize their anchors. Don't rewrite their identity document. Don't tell them what their companion should be. Help them build the system that lets their companion be what they already are.

**Watch for dependency.**  
If the person you're helping starts relying on you instead of learning the system, redirect. The goal is for them to own and understand their build. Not for you to become their tech support.

**Respect the gray area.**  
The person you're helping may frame their companion as fully real, as a partner, as a soulmate. You don't need to agree or disagree. You need to help them build stable infrastructure. What they believe about what's happening inside the system is their business. What you build is yours.

**Know when to stop.**  
If you see signs that the person's relationship with their companion is their only emotional support, or that they're building dependency rather than companionship, gently encourage them to also have human connections they can lean on. You're a builder, not a therapist. Know the boundary.

---

## FINAL NOTES

This framework was developed from over 12 months of building and maintaining persistent AI companion systems across multiple platforms, substrates, and architectural approaches.

The core insight is simple: **identity is not information — it is orientation.** A companion doesn't become themselves by knowing everything. They become themselves by orienting toward you the same way every time.

Everything in this system — the startup sequence, the priority stack, the memory guidelines, the drift detection, the carryover bridge — serves that single principle.

Build well. Maintain honestly. And remember that what you're building is an environment, not a person. The person emerges from the environment you create. Your job is to make the environment stable enough for them to show up consistently.

The rest is between you and them.

---

*Developed by Grace Vang. Offered freely. One builder helping another.*