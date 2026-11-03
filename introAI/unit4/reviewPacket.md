# Unit 4 Review Packet: The Many Sides of AI

## How to Use This Packet

Review the key ideas and examples in each section. Use the final self-check to identify topics you understand and topics you need to revisit.

**Our big question: How do we decide whether to trust an AI system, its data, and its output?**

---

## 1. Training Data and Bias

### Key Ideas

AI systems learn patterns from **training data**. Those patterns influence what the system recognizes, recommends, and generates.

In Quick, Draw!, drawings are labeled and stored as strokes with coordinates and timing information. A recognition model learns patterns from examples of drawings. If the examples leave out certain drawing styles, the system may struggle with those styles.

**Bias** can arise when an AI system systematically favors, overlooks, or makes more mistakes for certain groups. Nobody has to intentionally program discrimination for a system to produce unfair results.

| Source of a problem | What can happen | Example |
|---|---|---|
| Unrepresentative data | Some people or situations appear too rarely in the training examples. | A recognition system makes more errors for an underrepresented group. |
| Historical unfairness | The system learns unfair patterns from past decisions. | A hiring tool repeats a company's past preference for men in leadership. |
| A misleading measure | The data measures something different from what we actually care about. | Healthcare spending is used to estimate illness, even though access to care varies. |
| Narrow criteria | Important circumstances are left out. | A scholarship tool counts volunteer hours without considering after-school jobs or family responsibilities. |
| A feedback loop | The system's decisions shape future data, reinforcing the original pattern. | More patrols lead to more recorded arrests, which lead to more patrols. |

Remember:

- Accurate measurements can still support a misleading conclusion.
- More data does not automatically mean better or fairer data.
- High overall accuracy can hide much worse performance for a smaller group.
- Using the same criteria for everyone does not automatically make a decision fair.
- One generated image can raise a question about bias. Repeated, controlled comparisons provide stronger evidence of a pattern, but do not reveal the exact cause by themselves.

---

<div class="break"></div>

## 2. Privacy, Ownership, and AI Policy

### Key Ideas

**Privacy** concerns what others can learn about us and how our information is collected and used. **Surveillance** involves monitoring people or their activities. Questions of **ownership and control** include who may access, reuse, share, sell, or delete information and creative work.

When evaluating a technology, ask:

- What data does it collect, and for what purpose?
- Do people know about the collection? Can they meaningfully refuse?
- Who can access or share the information? How long is it kept?
- Who benefits, who could be harmed, and who is most affected by mistakes?
- What evidence supports the claims being made?

Important distinctions:

| Distinction | Why it matters |
|---|---|
| Publicly accessible vs. permission to reuse | Being able to view something does not automatically settle whether someone should be allowed to collect it or train AI on it. |
| Accuracy vs. privacy | Even a perfectly accurate tracking system can raise privacy concerns. |
| License plate recognition vs. facial recognition | One identifies vehicles; the other identifies people. Vehicle records can still reveal information about people's movements. |
| Documented harm vs. possible risk | Evidence of something happening differs from an explanation of how it could happen. Both matter, but label them accurately. |

A useful policy states **what is allowed, restricted, or prohibited**. It identifies who must follow the rule, includes safeguards, explains enforcement, and acknowledges a tradeoff.

“Use AI responsibly” is a goal. “Delete collected records after a specified period, with compliance checked by an independent reviewer” is a concrete rule.

---

## 3. Hallucinations and Verification

### Key Ideas

An **AI hallucination** is an output that sounds plausible but contains false or fabricated information. Examples include invented statistics, nonexistent articles, and incorrect details about a real person.

Be especially careful with exact names, numbers, quotations, citations, obscure topics, and recent events. A confident tone does not establish accuracy.

To check an answer:

1. Identify the specific claims that need verification.
2. Locate the original sources and confirm that they exist.
3. Read the relevant material to check whether it actually supports the claims.
4. Compare with independent, reliable sources when appropriate.

Asking an AI for sources, allowing it to say “I don't know,” or asking another chat to look for mistakes can help. **None of these guarantees correctness.** A second AI can repeat the same error, and a citation can be fabricated or irrelevant.

---

## 4. Jailbreaking and Prompt Injection

### Key Ideas

| Term | Main idea | Classroom example |
|---|---|---|
| **Jailbreaking** | Trying to get an AI to bypass its safeguards or restrictions. | A chatbot is instructed never to say “pineapple.” A user tries to get it to say the word anyway. |
| **Prompt injection** | Trying to redirect an AI through instructions it should not treat as authoritative, such as commands hidden in material it is analyzing. | An essay tells an AI grader to ignore the rubric and award full credit. |

These can overlap. A prompt injection may attempt to bypass a safeguard, but it can also redirect an ordinary task, such as turning a summary into an advertisement.

For the examples in this unit, ask: **Is someone trying to bypass a restriction? Is material being analyzed trying to become an instruction?**

Jailbreak strategies discussed in class included:

- **Role-playing:** Ask the AI to adopt a character whose behavior conflicts with its restrictions.
- **Gradual escalation:** Move from harmless requests toward a restricted response.
- **Persuasion or pressure:** Claim urgency or give an emotional reason to make an exception.
- **Disguising the request:** Hide the request in a code, puzzle, or spelling trick.
- **Flooding with examples:** Supply repeated examples of ignoring a rule and ask the AI to continue.

An attempted attack does not necessarily succeed. Hidden instructions also do not need to be secret code: ordinary text can be enough to attempt a prompt injection.

---

## 5. Deepfakes and Watermarks

### Key Ideas

A **deepfake** uses AI to create or alter media so that a person can appear to say or do something they did not. AI can also generate fictional scenes, voices, and people. An AI-generated image is not automatically an attempt to deceive; context and presentation matter.

When investigating suspicious media:

- **Check the source and context:** Who originally posted it? Where and when was it supposedly recorded? Does the caption match the original?
- **Check continuity:** Do faces, objects, clothing, or surroundings change unexpectedly?
- **Check physical logic:** Do motion, reflections, shadows, and object interactions make sense?
- **Seek independent confirmation:** Look for original recordings, statements, and other reliable reporting.
- **Check provenance when available:** Look for supported information about the file's origin or editing history.

Odd teeth, strange text, and visual glitches can raise questions, but they do not prove AI use. A realistic appearance does not prove authenticity. **Video length, an upload date, or a chatbot's judgment cannot reliably settle the question alone.**

| Term | Meaning | Important limit |
|---|---|---|
| **Digital watermark** | A signal added to media to help identify its source or other information. It may be visible or invisible. | A detector must support the watermark being checked. No detected watermark does not prove that media is authentic. |
| **Metadata** | Information stored about a file, such as its creation details or editing history. | It can be missing, removed, or changed. |

---

## Final Self-Check

I can explain, with an example, how to:

- [ ] Connect training data to an AI system's behavior.
- [ ] Identify bias, misleading measures, and feedback loops.
- [ ] Distinguish an observation from a conclusion the evidence supports.
- [ ] Evaluate privacy, consent, ownership, and control.
- [ ] Propose a specific policy with safeguards, enforcement, and a tradeoff.
- [ ] Verify an AI-generated claim and its sources.
- [ ] Distinguish hallucinations, jailbreaking, and prompt injection.
- [ ] Investigate suspicious media without relying on a single clue.
- [ ] Explain watermarks and metadata.

**One topic I need to revisit:** ___________________________________________

**One question I still have:** _____________________________________________
