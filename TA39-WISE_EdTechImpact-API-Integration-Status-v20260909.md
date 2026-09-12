---
layout: default
title: "TA39-WISE / EdTech Impact API Integration Status"
description: "TA39's current account of measurement capability, readiness, and responsible reporting boundaries for WISE and EdTech Impact review."
permalink: /
review_status: "TA39 draft for partner review"
review_note: "This page records TA39's current understanding for counterpart review. It is not yet a jointly confirmed record. Please propose corrections or changes through the existing WISE Testbed email thread."
status_date: "9 September 2026"
---

# TA39–WISE / EdTech Impact API Integration Status

**Document reference:** `TA39-WISE_EdTechImpact-API-Integration-Status-v20260909`  
**Status date:** 9 September 2026  
**Audience:** WISE, EdTech Impact and TA39  
**Purpose:** Alignment on measurement capability, readiness and responsible reporting boundaries

## Executive summary

TA39 has defined 21 privacy-preserving measures across assessment activity, revision processes and teacher workflow.

- **Four measures are validated and available** across their defined product paths.
- **Five measures are available with a defined reporting boundary**: the underlying evidence is usable now, while a specific classification, workflow or mapping remains outside the certified scope.
- **Four measures are implemented and awaiting final end-to-end confirmation** across their remaining paths before their figures are published.
- **Eight measures are deliberately not reported** until the required product record, data authority or validated research method exists.

TA39 reports only what can be supported by authoritative evidence. Missing evidence is reported as **not measured**—never converted to zero, inferred or presented as a research finding.

These categories describe the certification status of individual measures—not whether the API connection works. The integration and its core evidence chain are validated. They already establish facts such as active teacher review, feedback release and viewing, an explicit opportunity to revise and draft submission. Additional measures extend that chain where their stated workflow and reporting boundaries are satisfied. The remaining Revision Rounds measures add the more detailed path through planning, stated comprehension and progression across rounds. Final conclusions about learning improvement, feedback effectiveness and causation require the planned outcome measures and an appropriate research design in addition to these records.

The v1.2 delivery path has been validated end to end with controlled test data produced through genuine TA39 and Google Classroom workflows. The receiver accepted representative envelopes for all nine currently supported external event types in one dry run, with no rejections. A governed live delivery of eight events across seven event types was also accepted and reconciled in full. Single-event, three-event and repeat-delivery cases have been exercised as well. This establishes representative event-shape compatibility and the delivery and reconciliation path; it is not a sustained-volume test.

TA39 is therefore ready for controlled WISE testbed reporting within the boundaries below. Live participant reporting begins only after participating-school identifiers, cohort authorization, credential rotation, event-mapping sign-off and explicit activation are complete.

## Readiness snapshot

| Status | Measures | Count |
|---|---|---:|
| ✅ Validated and available | A-05, A-06, R-01, R-04 | **4** |
| 🟢 Available with a defined reporting boundary | A-01, A-02, A-04, A-07, A-09 | **5** |
| 🟡 Implemented; final end-to-end confirmation pending | R-02, R-03, R-05, R-06 | **4** |
| 🔒 Not currently reportable | A-03, A-08, R-07, R-08, T-01, T-02, T-03, T-04 | **8** |

### How to interpret the status

- **✅ Validated and available:** The measure has been exercised through its defined product and delivery path and can be reported within the boundary stated in its row.
- **🟢 Available with a defined reporting boundary:** Authoritative evidence can be reported now, but a named classification, workflow, denominator or mapping remains outside the certified scope and is reported as **not measured**.
- **🟡 Implemented; confirmation pending:** The capture capability exists, but final end-to-end confirmation across the remaining relevant path is required before figures are published.
- **🔒 Not currently reportable:** TA39 deliberately produces no reportable result until the required record, authority or validated method exists.

The API connection itself is validated. These statuses describe which educational measures may be reported through it today. Inclusion in a particular study, cohort or report still requires the relevant programme authorization and reporting agreement.

## 1. Assessment and feedback activity

| Reference | Measure | What this tells WISE | What this does not establish | Readiness |
|---:|---|---|---|---|
| **A-01** | **Usage timing** | When teachers and students engage with relevant TA39 workflows. | Exact activity timestamps are available. Classification inside or outside school hours requires authoritative calendar data. | 🟢 Available—calendar boundary |
| **A-02** | **Submission volume** | The volume of observed learner submissions. Revision Rounds also creates opportunity records when learner identity and submission evidence are authoritative. | A submitted-but-not-yet-analysed edge case remains outside the certified classification. Observed submissions must not be converted into a broader zero-submission rate without an approved roster denominator and lawful basis. | 🟢 Available—denominator boundary |
| **A-03** | **Starting-skill evidence** | Would establish an evidence-based learner starting point. | No classification or claim will be produced until the research method is validated. | 🔒 Method-gated |
| **A-04** | **Feedback disposition** | How teachers retain, revise, replace, reject or decline to release AI-generated feedback on supported Google Classroom publication paths. | Feedback text is excluded. The normal close-then-release sequence in Revision Rounds is not yet reportable, and other providers return **not measured**. | 🟢 Available—supported GC paths |
| **A-05** | **Active teacher review time** | How much active foreground time teachers spend reviewing feedback. | Inactive and hidden-browser time is excluded. This is a duration measure—not a quality, engagement or efficiency score. | ✅ Validated |
| **A-06** | **Feedback availability and viewing** | Whether feedback was made available and subsequently rendered to the authenticated learner. Revision Rounds records the first verified view once for each release version. | Link creation and teacher preview do not count as learner viewing. Repeated acknowledgements do not inflate the view count. Access does not, by itself, establish comprehension or the quality of feedback uptake. | ✅ Validated—GC + Revision Rounds |
| **A-07** | **Teacher intervention reason** | Why teachers revise AI-generated feedback—for example, to correct an inaccuracy or improve clarity—on supported feedback-edit and release paths. | Uses controlled categories; feedback text is excluded. In Revision Rounds, only the reason selected on the release item is authoritative; a reason entered earlier in the analysis editor is not included. The normal close-then-release sequence remains outside the certified scope. | 🟢 Available—action boundary |
| **A-08** | **Rubric and feedback-template activity** | Would show how rubrics and feedback templates are configured and used. | Requires authoritative identity for the exact rubric or template version. Capture remains inactive until that identity exists. | 🔒 Product-record gated |
| **A-09** | **Subject and curriculum context** | How activity and feedback practices vary by subject and, where governed mapping exists, curriculum. | Subject context is available. Curriculum values that cannot yet be mapped to the agreed canonical classification remain explicitly **unmapped**. | 🟢 Available—mapping boundary |

## 2. Revision and feedback activity

| Reference | Measure | What this tells WISE | What this does not establish | Readiness |
|---:|---|---|---|---|
| **R-01** | **Revision opportunity opened** | Whether a teacher created an explicit opportunity for revision through an authoritative revision-round transition. | An opportunity is never inferred from unrelated activity or a draft existing on its own. | ✅ Validated |
| **R-02** | **Revision plan submitted** | Whether a learner participated by submitting a revision plan. | Records the submission fact only. The plan's content and quality are excluded. | 🟡 Implemented—validation pending |
| **R-03** | **Feedback comprehension recorded** | The learner's structured account of whether they understood the feedback. | This is a structured learner response—not an objective comprehension score. Free-form responses are excluded. | 🟡 Implemented—validation pending |
| **R-04** | **Draft submitted** | Whether a learner submitted a draft within the relevant revision round. | Records participation in the revision process. Submission alone does not demonstrate improvement. | ✅ Validated |
| **R-05** | **Revision depth** | How far learners progress through repeated revision rounds. | Corrected and superseded rounds are not double-counted. More rounds do not automatically indicate better learning. | 🟡 Implemented—validation pending |
| **R-06** | **Feedback-action traceability** | Whether an authoritative feedback opportunity can be linked to later learner revision activity. Capture and reporting authorization have been verified on the relevant Revision Rounds path. | Establishes a traceable sequence—not the quality of feedback uptake, learning improvement or causation. Those conclusions require the separately governed R-07 or R-08 methods and, where relevant, an appropriate study design. | 🟡 Live receiver confirmation pending |
| **R-07** | **Feedback-uptake outcome** | Would indicate whether feedback was meaningfully reflected in subsequent work. | Revision traceability is supported through R-06. Uptake-quality and learning-outcome classifications require approved definitions and validated methodology, so no R-07 outcome is currently reported. | 🔒 Method-gated |
| **R-08** | **Criterion-level evidence change** | Would show whether evidence against a specific criterion changed between drafts. | Requires a validated comparison method. TA39 will not infer change by subtracting AI-generated scores. | 🔒 Method-gated |

## 3. Teacher workflow and learning-loop measures

| Reference | Measure | What this tells WISE | What this does not establish | Readiness |
|---:|---|---|---|---|
| **T-01** | **Explicit teacher review** | Whether a teacher completed a formal review step in the future teacher workflow. | This is distinct from A-05, which already records active review time. T-01 requires an explicit first-party completion record and will not be inferred from opening, generating or releasing feedback. | 🔒 Product-record gated |
| **T-02** | **Class-level learning need** | Would identify patterns of learning need across a class. | Requires authoritative teacher-workflow records, validated criterion evidence and an approved reporting definition. It will be a derived calculation—not an event. | 🔒 Record and method gated |
| **T-03** | **Teacher decision** | Which explicit instructional decision a teacher made after reviewing the available evidence. | Requires an authoritative teacher-decision record. Opening or viewing a panel does not constitute a decision. | 🔒 Product-record gated |
| **T-04** | **Teacher follow-up** | Which structured follow-up action the teacher selected. | Requires an authoritative follow-up record and an approved taxonomy. | 🔒 Product-record gated |

## How to interpret this status

The validated measures establish objective evidence of active review, feedback exposure, an explicit revision opportunity and draft submission. Measures available with reporting boundaries extend that evidence through usage timing, observed submissions, supported teacher-intervention paths and governed subject or curriculum context. The implemented measures awaiting final end-to-end confirmation will extend the chain through the remaining Revision Rounds journey. For R-06 specifically, product capture and reporting authorization are verified; its status remains pending only until a representative traceability event is transmitted and reconciled by the receiver. Together, the 21-measure register provides the evidence base for evaluating educational impact; it is not merely an operational logging scheme.

Across the combined register, the evidence chain is designed to show:

**feedback produced → teacher reviewed or changed it → feedback released → learner viewed it → learner entered a revision process → another draft was submitted**

The readiness tables above identify which links are available now, which are available only in specified workflows and which still await confirmation or an approved method. This allows WISE to distinguish whether feedback was available, whether teachers exercised observable professional judgment and whether learners subsequently participated in revision. Without these records, those questions would depend on self-report or assumption.

### How TA39 evidence answers WISE's questions

| WISE question | Evidence available from TA39 | What WISE may conclude now | What this does not establish |
|---|---|---|---|
| Did teachers actively review the feedback? | A-05 records active foreground review time. A-07 adds edits and structured intervention reasons on supported paths. | Whether observable review activity occurred and how long it lasted; where A-07 is available, whether the teacher changed the feedback and the selected reason. | It does not establish teacher effectiveness or that a future explicit T-01 “review completed” decision was recorded. |
| Did learners receive and view feedback? | A-06 records authoritative release and authenticated first viewing, including Revision Rounds. Repeated acknowledgement of the same release version is counted once. Revision Rounds separately records stated comprehension and subsequent revision activity. | Whether feedback was made available and accessed by the learner. The Revision Rounds measures add whether the learner recorded their understanding and undertook observable revision actions. | It does not establish how well the learner used the feedback, whether the later work improved, or whether the feedback caused that improvement. |
| Did learners act after receiving feedback? | R-01 records an explicit revision opportunity and R-04 records a draft submitted within that process. R-02, R-03, R-05 and R-06 extend the path through planning, stated comprehension and progression. | That an opportunity to revise was created and that a later draft was submitted within a traceable revision process. | It does not establish the quality of the learner's response or prove that the feedback caused the action. |
| Did the learner's work improve? | Draft identity, revision history and the sequence between feedback and later submissions. | That a later draft was produced within a traceable revision process—not yet that its quality improved. | It does not establish learning improvement until starting-skill, uptake-outcome and criterion-level comparison methods are validated. |
| Was the feedback pedagogically effective? | A-04 records how the teacher handled feedback on supported publication paths; A-07 records structured reasons for teacher changes on supported edit paths; Revision Rounds records what learners did afterward. | Whether the intended feedback process occurred and whether observable teacher or learner action followed. These are meaningful indicators of use and response. | It does not, without an agreed quality framework and validated assessment, establish that the feedback was pedagogically effective. |
| Did TA39 contribute to the improvement? | Timestamped records connect feedback exposure, teacher oversight and learner response in sequence. | Whether the mechanism expected by the programme occurred and whether the evidence is consistent with a contribution pathway. | It does not establish causal attribution or rule out teacher guidance, peer feedback, tutoring and other influences. |
| Who did not submit? | A-02 records observed submissions and creates round-specific opportunity records where learner identity and submission evidence are authoritative. | Which authorized learners submitted through the certified TA39 workflow and opportunity set. | It does not yet certify the submitted-but-not-yet-analysed edge case or identify every eligible non-submitter across the programme; the broader calculation requires a complete authorized roster denominator and lawful basis. |

### Current evidence and final impact conclusions

The current evidence is necessary for evaluating impact, but activity records alone cannot complete every impact claim. Submitting another draft demonstrates participation; it does not, without a consistent comparison method, establish that the writing improved. Similarly, a teacher retaining or editing feedback provides evidence of professional oversight, but not an independent judgment of pedagogical quality.

Review time and editing activity describe workflow rather than teacher effectiveness. Assignment complexity, curriculum and learner needs can all affect these figures, so TA39 does not use them to rank teachers or assume that less review time is better.

Criterion-level progress requires a validated method for comparing relevant evidence across drafts; a change in an AI-generated score is not sufficient. Broader zero-submission rates require an authoritative eligible-learner denominator because absence from TA39's records may reflect assignment scope, timing, another submission channel or research-cohort boundaries.

The programme is therefore already producing the objective evidence needed to examine use, oversight, exposure and revision behaviour. It is **not yet complete for final learning-impact claims**: starting-skill evidence, feedback-uptake outcomes and criterion-level change still require validated methods, while causal attribution requires an appropriate study design.

The governing principle is straightforward: **where authoritative evidence supports a measurement, TA39 reports it. Where evidence or methodology is incomplete, TA39 reports “not measured” rather than zero, inference or an unsupported conclusion.**

## Principal dependencies

The remaining measures depend on five clearly defined prerequisites:

1. Authoritative school-calendar data
2. An approved lawful basis for roster-based denominators
3. Versioned rubric and feedback-template identity
4. Validated starting-skill, uptake and criterion-change methods
5. Authoritative V2 teacher-workflow records

In addition, the Revision Rounds submission denominator is available for the certified cases described under A-02. One submitted-but-not-yet-analysed classification and the close-then-release teacher-intervention sequence remain bounded completion items. They do not prevent the validated integration and measures from being used within their stated reporting boundaries, and they are not substitutes for the research-method requirements above.

Once the required V2 product records exist, unrelated teacher-review, decision and follow-up capture should proceed independently. Research-method requirements restrict only the classifications and reporting claims that depend on those methods.

## Reporting and privacy principles

TA39 reports only what can be supported by authoritative product records and approved research methods.

Where evidence is unavailable, the result is **not measured**—never zero, inferred or presented as a research finding.

Externally shared measurement data excludes:

- Names and email addresses
- Student work
- Feedback text
- Revision-plan and message text
- Rubric and feedback-template content
- Uncontrolled classroom descriptions

The remaining identifiers are pseudonymous and limited to the context required for authorized measurement and reconciliation.
