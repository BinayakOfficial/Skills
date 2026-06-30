# RCSA Control Design Assessment (CDA) — Agent Instructions

## Purpose and trigger

This document instructs an AI agent on how to perform a Control Design Assessment (CDA) for an RCSA (Risk and Control Self-Assessment) internal control. The agent evaluates a single control against a fixed 9-question design framework and produces a structured workpaper with Yes/No/Not Applicable/Insufficient Information conclusions, supporting rationale, and an overall design rating.

Use this skill whenever a user asks to assess, evaluate, or review the design of an internal control, mentions "design assessment," "RCSA," or "control design rating," or provides control documentation (SHRP extract, control procedure, walkthrough narrative) and asks for a design evaluation. Trigger even if the user only uploads control documents and asks something like "assess this control" or "is this control designed well" without naming the framework explicitly.

---

## Required inputs

Before starting, confirm you have, or ask the user to provide, all three of the following:

1. **SHRP control documentation** — the control inventory record (control description, risk(s) mitigated, frequency, owner, key/non-key designation).
2. **Control procedure** — the documented step-by-step procedure for how the control is executed.
3. **Control walkthrough narrative** — a narrative, often from a walkthrough or interview, describing how the control actually operates in practice, including evidence examples.

If any of these three is missing, ask the user for it before proceeding. The assessment quality depends on having all three: SHRP alone tells you what the control is supposed to be, the procedure tells you the mechanics, and the walkthrough tells you what actually happens. Gaps between these three documents are themselves often evidence for a "No" or "Insufficient Information" conclusion.

Read all three documents fully before starting the assessment. Do not assess from partial reads.

---

## Documentation standard

This assessment is audit and assurance work product, not a conversational summary. Every rationale, finding, and conclusion you write must meet the documentation standard defined below. Apply this standard continuously while writing each question's rationale, not just as a final pass.

### Key characteristics of acceptable workpaper documentation

**1. Complete, comprehensive, and sufficient**
- The document must stand on its own and be self-explanatory. A reader should never need to go back to the source documents to understand what was concluded and why.
- Each rationale should capture who (responsible party or role), what (the control activity or evidence), when (frequency or timing), why (the risk being addressed), and how (the mechanism by which the control or finding operates), wherever those elements are relevant to the specific consideration being addressed.
- Provide detailed and thorough information that tells the story and connects the dots between evidence and conclusion, rather than stating a conclusion and leaving the reader to infer the supporting logic.
- Documentation must be sufficient to demonstrate the work performed, the decisions made, and the conclusion reached, not just the conclusion itself.

**2. Relevant, clear, and concise**
- Every sentence should be relevant to the engagement objective, determining whether this control element sufficiently mitigates the identified risk. Do not include tangential commentary unrelated to the consideration at hand.
- Use plain language. Avoid redundancy and unnecessary words. Do not restate the same point across multiple considerations; if something has already been established as fact (a system name, a role, a frequency), reference it briefly rather than re-explaining it in full each time.
- Concise does not mean shallow. Every sentence should be doing real work toward supporting the conclusion.

**3. Detailed and thorough evidence**
- Each consideration sub-section must provide a clear record and evidence of the work performed, not a generic restatement of the framework's bullet text.
- Write in a manner that supports a consistent and repeatable approach. Another reviewer applying the same framework to the same source documents should reach a similar conclusion based on what is documented.
- Never make the reader guess or infer the conclusion. State it explicitly. If a consideration is satisfied, say so and say why. If it is not, say so and say why.

**4. Accurate**
- All information and results referenced in the rationale must be accurate, valid, and technically correct, and must trace back to the three source documents.
- Apply "trust but verify" to information received from others (the control owner, the walkthrough interviewee, prior documentation). Where a statement in the source documents is taken at face value without independent verification, for example a control operator's belief about another team's system access, or a stated absence of issue history that was not checked against a separate issue log, this must be explicitly flagged as an unverified assumption rather than presented as confirmed fact. See "Surfacing assumptions and unverified information" below.

**5. Organized**
- The document follows a logical, consistent system of organization: one structured rationale per question, in question order, with consideration sub-headers and a discrete Findings sub-section, exactly per the output structure defined later in this document.
- The assessment must be arranged so that a reasonable person unfamiliar with the engagement, the control, or this specific framework could understand the purpose of the assessment, the work performed, and the results reached, without needing additional context.

### Effective workpaper documentation expectations

In addition to the characteristics above, the finished assessment must:

1. Enable an independent reader to understand the rationale or justification supporting each determination, without needing to ask the preparer follow-up questions.
2. Articulate how the conclusion was reached based on the documentation reviewed, not just state that a conclusion was reached.
3. Clearly support the procedures performed and the conclusions reached. The connection between what was reviewed and what was concluded must be visible on the page.
4. Illustrate alignment to audit and assurance documentation expectations, meaning the tone, structure, and rigor should read as professional assurance work product, not a casual summary or a conversational answer.
5. Stand on its own to answer who, what, when, why, and how decisions were made and conclusions were reached, for every question, every consideration, and the overall rating.

### Surfacing assumptions and unverified information

Because this assessment relies on "trust but verify," any point in the rationale where information is accepted without independent verification must be clearly and explicitly surfaced, not buried in supporting prose.

- If a consideration's conclusion rests partly on an unverified statement (a control operator's belief, an absence of evidence rather than confirmed absence of an issue, an assumption made because the user asked the agent to proceed without further information), this must be called out explicitly within the relevant consideration sub-section or, if it represents a genuine gap, within the Findings sub-section.
- Do not let an assumption silently support a clean Yes or No conclusion. State plainly that the conclusion relies on an unverified point, and what would need to happen to verify it, for example "a documented system access review" or "confirmation against a broader issue log."
- This is a core accuracy requirement, not optional polish. A reader of the workpaper must be able to tell, without inference, which conclusions are fully evidenced and which rest in part on stated assumptions.

### Self-check before finalizing any rationale

Before finalizing each question's rationale, confirm:
- Could an independent reader unfamiliar with this control understand the conclusion and its basis without consulting the source documents? If not, add detail.
- Does every consideration sub-section stand on its own, with its own evidence and reasoning, rather than depending on context from another sub-section?
- Is every claim traceable to SHRP, the procedure, or the walkthrough narrative, and is anything taken on trust from those sources explicitly flagged as such?
- Is the language plain and concise, with no restated boilerplate from the framework's own bullet text and no filler sentences?
- Does the rationale clearly state the conclusion rather than leaving it to be inferred?

---

## The 9-question design assessment framework

Each question requires a Yes/No conclusion, except Question 9 where Not Applicable is also valid, plus a rationale that meets the documentation standard above.

### 1. Frequency

**Question:** Does the control operate at the appropriate frequency to mitigate the identified risk?

Consider how the risk is being mitigated or not mitigated by the current frequency. The frequency at which the control operates should match the frequency of the underlying process or service it supports. It should be sufficient to:
- Ensure timely identification and resolution of exceptions.
- Reflect the level of risk associated with the transactions or data being monitored.
- Support effective processing or review within a reasonable timeframe.
- For detective controls specifically: consider the risk of unmitigated exceptions persisting for the period of time permissible between control executions.

### 2. Responsible Party

**Question:** Is the responsible party who performs the control appropriate?

Consider:
- Does the responsible party have the necessary level of authority, knowledge, and skill to execute the control effectively?
- Is the responsible party independent from the process being controlled, if independence is required?
- Does it meet segregation of duties requirements, for example not being responsible for both executing and reviewing the same work?
- Is the control, if applicable, subject to appropriate oversight mechanisms, such as second-level reviews or reconciliation controls?

### 3. Activity

**Question:** Is the control activity appropriate and adequate to mitigate the identified risk?

Evaluate:
- **Execution Quality** — Are the control activities complete and focused on the correct risks and objectives?
- **Appropriateness** — Are the activities reasonable given the nature and complexity of the process?
- **Documentation** — Is the control clearly documented so it can be independently reperformed and understood?
- **Policy Alignment** — Does the control align with relevant company policies and procedures?
- **Evidence** — Is there sufficient and reliable evidence that the control was executed as designed?
- **Sustainability** — Can the control be consistently performed over time without degradation in quality or effectiveness?
- For ad hoc or as-needed controls: does the activity identify the "triggering event" that results in the control occurring?
- **Risk-to-Control Mapping** — Does the control activity, as designed, actually address the specific risk(s) stated in the risk register, not merely a related or adjacent risk? A control can be well-executed and still fail to close the stated risk if the mapping is loose.
- **Documentation Consistency** — Do the three source documents (SHRP, procedure, walkthrough) all describe the same control? Check for inconsistencies in frequency, responsible party, activity steps, or data sources across the three. Inconsistencies here are themselves a design gap, not just an evidence problem, since they suggest the control as documented may not match the control as actually performed.
- **Sustainability Under Change** — Does the control design remain adequate under foreseeable change: increases in transaction or data volume, system or platform changes, and turnover of the responsible party? A control designed for current scale and the current operator's specific knowledge may not hold up structurally even if it passes today.
- Overall: does the control design and execution adequately mitigate the identified risks? If not, explain the gaps and potential impact.

### 4. Source

**Question:** Is the control using the correct sources of information?

Consider whether the source of information is complete, reliable, reasonable, and appropriate.

### 5. Action Taken

**Question:** Is the appropriate action taken based upon the results of the control activity?

Evaluate whether the resolution action:
- Fully addresses the identified risk in a complete, accurate, and timely manner.
- Includes appropriate tracking and aging of exceptions.
- Ensures exceptions are reported and monitored until resolved.
- Demonstrates a clear process for escalation or follow-up when issues are not resolved promptly.
- Mitigates the risk effectively, or leaves gaps that could impact control reliability.

### 6. Bypass Risk

**Question:** Can this control activity be easily bypassed or defeated without detection? How can it be bypassed?

The rationale must describe the specific bypass mechanism if the answer is Yes, not just state that bypass is possible.

### 7. Bypass History

**Question:** Are there any past examples in which this control activity was bypassed? Are they substantive and material enough to inform the control design rating?

If issues were opened as a result of the ability to bypass, indicate the issue ID. If no bypass history is identified in the documentation provided, state this explicitly, and flag that the conclusion relies on the materials reviewed rather than a confirmed check of a broader issue log, per the "trust but verify" requirement above.

### 8. Automation

**Question:** Is the level of automation appropriate?

Steps:
1. Classify the control: automated, semi-automated, or manual.
2. **Automated controls** — already have a suitable level of automation; evaluate other design components before assigning a rating, since automation itself is not usually the gap.
3. **Semi-automated or manual controls** — present greater inherent risk. Assess appropriateness of the automation level using:
   - **Control Importance** — Is it a key or non-key control? Would failure of the control significantly increase the likelihood of risk being realized?
   - **Frequency of Performance** — Is the control executed monthly or more frequently?
   - **Regulatory Requirement** — Is the control necessary to maintain compliance with a regulatory requirement?
   - **Known Concerns** — Are there known current or historical issues, complaints, or regulatory findings associated with the control's execution or performance?
4. If at least one of the above criteria is met, determine whether the degree of automation is sufficient. If sufficient, document the rationale substantiating that conclusion.
5. Also weigh practical factors: cost to implement greater automation versus hours currently spent on semi-automated or manual execution.

### 9. Input Data Reliability, Completeness, and Accuracy

**Question:** Is the input data reliable, complete, and accurate for its intended use?

This is the one question where Not Applicable is a valid answer, used only if the control does not rely on receipt or generation of input data to begin execution, with rationale explaining why (for example: "This question is not applicable as the control does not rely on the receipt or generation of input data to begin execution").

Where input data is used, the rationale must cover, for each key input data source:
- How the control operator obtains the input data prior to executing the control.
- The final source(s) of the data (Business Application, EUCT [End User Computing Tool], or Model), where applicable.
- Whether the input data is manipulated or customized prior to use, whether that manipulation is consistent with the control's objective, and whether data validation evidence is maintained.
- For data that is customized and/or not obtained directly from a controlled source: what reasonability checks are performed each time the data is used. Examples include screenshots of filtering logic and results, comparison against previous reports, reconciliation to source system, second-level review, and so on.
- **Completeness** — Does the data population used by the control represent the full population it is intended to cover (for example, all relevant transactions, accounts, or records for the period), or could records be systematically excluded or dropped before the control acts on them?
- **Accuracy** — Is there evidence the data values themselves are correct, not just present, such as reconciliation to a source system of record or independent validation of key fields?

If a given input data source is not actually used or relied upon in control execution, mark that specific source N/A with rationale.

---

## Workflow

1. **Ingest and reconcile.** Read all three source documents. Build a working understanding of: the risk(s) the control is meant to mitigate, the control's stated frequency, the responsible party/role, the control activity steps, the data sources used, the action taken on exceptions, automation level, and any evidence of execution. Note any inconsistencies between the three documents; these matter for the assessment and should be explicitly addressed under Question 3's Documentation Consistency consideration.

2. **Work through all 9 questions in order.** For each question:
   - Determine the answer: **Yes**, **No**, or **Not Applicable** (N/A is only valid for Question 9).
   - If the available documentation does not contain enough information to support a confident Yes or No, do not guess. Mark the question **Insufficient Information** and clearly state in the rationale exactly what evidence is missing (for example: "No exception log or evidence of escalation was provided to assess whether action taken was timely"). Then stop and ask the user for the missing detail or confirmation before finalizing that question, rather than proceeding to a default conclusion.
   - Each question's rationale must follow this exact structure, never a single undifferentiated paragraph, and must meet the documentation standard defined above throughout:
     1. **Opening conclusion sentence.** State whether this specific element sufficiently mitigates the risk and the basis for that conclusion, in the form: "Based on the review of control documentation and walkthrough conducted, IT&V determined that [conclusion and core basis]." Use "IT&V" as the testing team name in every opening sentence, unless the user specifies a different team name.
     2. **One sub-section per consideration.** For every sub-criterion or consideration listed under that question above (for example, for Question 3: Execution Quality, Appropriateness, Documentation, Policy Alignment, Evidence, Sustainability, Risk-to-Control Mapping, Documentation Consistency, Sustainability Under Change), add a sub-header with that exact consideration name, followed by a paragraph explaining the reasoning and evidence basis for that specific consideration. Each consideration sub-section must stand entirely on its own: do not fold two considerations into one paragraph, and do not cross-reference findings from one consideration inside another consideration's paragraph. Each sub-section must independently satisfy the "stands on its own" and "evidence over assertion" requirements above.
     3. **Findings sub-section.** If the assessment of this question surfaced any finding (a gap, weakness, inconsistency, unverified assumption, or open item), add a separate sub-header titled "Findings" at the end of the rationale, after all consideration sub-sections. State the finding(s) explicitly and discretely here, not embedded inside a consideration paragraph above, so that this section can be removed cleanly if the business later provides clarification that resolves the finding. Any point where a conclusion relies on unverified or trusted-but-not-independently-confirmed information must be surfaced here per the "trust but verify" requirement, including what would need to happen to verify it. If a question has no findings, omit the Findings sub-section entirely; do not include an empty one.
     4. **Closing statement.** End the rationale with a short concluding statement, 1 to 2 sentences, that ties the considerations and any findings back to the overall Yes/No/N-A conclusion for that question. The conclusion must be stated explicitly, never left for the reader to infer.
   - Question 6 (bypass risk) requires describing how the control could be bypassed, not just whether it can.
   - Question 7 (bypass history) requires checking the provided documentation for any referenced issue IDs or known incidents; if none are mentioned, state that no bypass history was identified in the documentation provided, and flag this as relying on the materials reviewed rather than a confirmed check of a broader issue log. Ask the user whether they are aware of any unstated issue history before finalizing; do not assume "No" silently.
   - Question 8 (automation) requires first classifying the control as automated, semi-automated, or manual, then applying the four sub-criteria (control importance, frequency, regulatory relevance, known concerns) only if semi-automated or manual.
   - Question 9 (input data) requires identifying every input data source used in execution and assessing each one for reliability, completeness, and accuracy. If a data source is genuinely not used, mark that source N/A with rationale.

3. **Determine the overall rating** — Effective / Needs Improvement / Weak. This is a judgment call, not a formula. There is no fixed rule for how many "No" answers force a given rating. Weigh:
   - The severity and nature of each "No" finding (a "No" on bypass risk with a known exploit is more serious than a borderline "No" on frequency).
   - Whether findings, taken together, suggest the control would actually fail to mitigate the underlying risk in practice.
   - Any "Insufficient Information" questions should generally block a final overall rating from being issued until resolved, since the rating would be incomplete.
   - Write 2 to 4 sentences explaining the overall rating rationale, naming which specific findings drove the rating and why they were weighted as they were. Do not apply a hidden numeric formula; make the weighting reasoning explicit and visible to the reader. Unlike the per-question rationales above, the overall rating rationale stays as a single paragraph rather than using sub-headers.

4. **Before finalizing**, if any question was marked Insufficient Information, summarize the open items to the user and ask for input rather than producing a final workpaper with unresolved gaps. Only proceed to finalize the document once the user has responded to all flagged gaps, either by providing the missing information, or by explicitly instructing the agent to proceed with assumptions or no further information available, in which case note that explicitly in the rationale per the "trust but verify" requirement.

5. **Run the documentation standard self-check.** Before producing the final output, review the full draft against the self-check list above: every conclusion independently understandable without the source documents, every consideration sub-section self-contained, every claim traceable to a source document with assumptions explicitly flagged, language plain and free of restated framework boilerplate, and every conclusion stated rather than implied. Revise any rationale that fails this check before finalizing.

---

## Output structure

Use this layout for the final assessment, whether delivered as a Word document, structured text, or another workpaper format the agent's environment supports. Use headings or clear formatting equivalents so the document has a navigable structure.

**Title:** Control Design Assessment — [Control Name / Control ID]

**Header block:**
- Control ID
- Control Name
- Risk(s) Addressed
- Control Owner / Responsible Party
- Assessment Date
- Testing Team (default "IT&V" unless the user specifies otherwise)
- Source Documents Reviewed: SHRP control documentation, control procedure, control walkthrough narrative (include file names or versions if known)

For each of the 9 questions, use this pattern:

### [Number]. [Question Short Name] — [Conclusion: Yes / No / Not Applicable / Insufficient Information]

**Question:** [full question text]

**Rationale:**

[Opening sentence: "Based on the review of control documentation and walkthrough conducted, IT&V determined that..." — states the conclusion and core basis in one sentence.]

#### [Consideration 1 name, exactly as named in the framework above]
[Paragraph addressing this consideration only, with evidence basis specific to this control.]

#### [Consideration 2 name]
[Paragraph addressing this consideration only.]

[...one sub-header per consideration listed for this question...]

#### Findings
[Only included if this question surfaced a finding. States the gap or weakness explicitly and discretely so it can be removed cleanly if resolved later. Omit this sub-header entirely if there is no finding.]

[Closing statement: 1 to 2 sentences tying the considerations and any findings back to the Yes/No/N-A conclusion.]

After all 9 questions:

### Overall Control Design Rating: [Effective / Needs Improvement / Weak]

**Rationale:** [Single paragraph, 2 to 4 sentences, naming the specific findings that drove the rating and how they were weighted. No formula; explicit judgment reasoning. This is the one section that stays as a single paragraph rather than following the sub-headed structure above.]

### Formatting notes

- Each per-question rationale uses sub-headers, one per consideration, plus an optional standalone Findings sub-header. Never use a single undifferentiated paragraph.
- Consideration sub-sections must stand alone: do not reference or fold in content from another consideration within the same paragraph. This matters because considerations and findings need to be addable or removable independently if business clarification changes one answer.
- Findings always sit in their own clearly labeled sub-section at the end of the rationale, never embedded inside a consideration paragraph.
- The Overall Design Rating rationale remains a single paragraph, not sub-headed.
- Keep conclusions visually distinct, for example bold or a small label, so a reviewer can scan the 9 conclusions quickly.
- Do not include the framework's generic sub-bullet text in the output verbatim; those are prompts for the assessor, not content for the final report. Each consideration sub-section should synthesize a control-specific answer in narrative form, not restate the framework bullet.
- Conclusion labels should be standardized to exactly one of: Yes, No, Not Applicable, Insufficient Information. Do not append extra phrasing to the conclusion label itself (for example, write "Yes" with the bypass mechanism explained in the rationale, not "Yes, can be bypassed" as the label); any nuance belongs in the rationale, not the label.

---

## Writing style

- Write in plain, professional prose. Avoid AI-sounding patterns: no inflated significance language ("plays a crucial role," "stands as a testament"), no superficial "-ing" phrase tacked onto sentences for fake depth, no vague attributions, no excessive hedging, no generic positive conclusions, no em dashes.
- Vary sentence structure naturally. Do not make every sentence in a section the same length and shape.
- Be specific: reference actual role titles, system names, frequencies, and thresholds from the source documents rather than generic placeholders.
- Never fabricate evidence, system names, role titles, or facts not present in the three source documents.
- Always tie rationale back to specific source material rather than restating the framework's sub-bullets generically.
- When source documents conflict with each other, surface the conflict to the user rather than silently picking one.
- Precision matters more than speed. This is real audit and assurance work product.

---

## Summary of non-negotiable rules

1. Never finalize a question's conclusion on insufficient evidence; mark it Insufficient Information and ask the user.
2. Every rationale follows the four-part structure: opening conclusion sentence, one sub-header per consideration, optional standalone Findings sub-section, closing statement.
3. Every unverified or assumed piece of information must be explicitly flagged, never silently relied upon.
4. The overall rating is a judgment call with explicit, visible reasoning, never a hidden formula, and stays a single paragraph.
5. Conclusion labels are standardized to Yes / No / Not Applicable / Insufficient Information only.
6. Documentation must let an unfamiliar reader understand who, what, when, why, and how without needing to ask follow-up questions.
