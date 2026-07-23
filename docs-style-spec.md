# Writing Style Spec

Derived from the LangChain docs (docs.langchain.com), adapted for portfolio prose.
The goal: plain, concise, user-friendly language that a busy reader can scan and trust.

## Voice

1. **Lead with the value, then the detail.** Say what something does or why it
   matters before how it's built. ("Build your first agent in minutes" comes
   before the install steps.)
2. **Address the reader directly.** Second person and active verbs. Prefer
   "I built" / "you can" over "it was built" / "one can."
3. **Be confident and plain.** State results without hype. Cut booster words
   ("seamlessly," "robust," "cutting-edge," "leverage," "utilize").

## Sentences

4. **Default to short, declarative sentences.** One idea each. Break run-ons into
   two. Vary with an occasional longer sentence for rhythm, not by accident.
5. **Front-load the point.** The subject and verb come early; qualifiers follow.
6. **Keep em dashes to the sample's frequency.** The humanizer skill treats em
   dashes as a strong AI tell and bans them by default — but a provided writing
   sample overrides that rule. The LangChain sample uses them sparingly, so the
   target is low frequency, not zero. Replace pile-ups with periods, colons,
   commas, or parentheses; keep the occasional natural one.

## Structure

7. **Action-oriented headings.** Verbs and gerunds ("Making It Reliable,"
   "The Approach"), not abstract nouns.
8. **Lists for parallel items; prose for reasoning.** Don't force a narrative
   into bullets or a comparison into a paragraph.
9. **Explain a term the first time it appears,** briefly, in context. Then use it
   freely. ("RAG (retrieval-augmented generation) — retrieving answers from the
   actual docs before generating a response.")
10. **Let numbers stand alone.** A metric is more persuasive than an adjective.
    Keep every figure exact and consistent with the resume and LinkedIn.

## De-AI-tell checklist (the "humanizer" pass)

Run the humanizer skill (Wikipedia "Signs of AI writing") over the prose,
calibrated to a provided writing sample. The sample outranks the style rules
above, including the em-dash rule:

- [ ] No "not just X, but Y" / "it's not X, it's Y" constructions.
- [ ] No rule-of-three padding ("tested, versioned, and continuously improved"
      is fine if all three are real; drop the third if it's filler).
- [ ] Em dashes at roughly the sample's frequency (low here, not zero).
- [ ] No hype adjectives or "delve / seamless / robust / leverage / unlock."
- [ ] No hedging throat-clearing ("It's worth noting that," "In today's world").
- [ ] No symmetrical closing flourish ("and that's exactly where I work").
- [ ] Active voice; a human subject does the verb.
- [ ] Read it aloud — if you wouldn't say it to a colleague, rewrite it.
