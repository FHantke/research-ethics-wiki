---
weight: 1000
bookFlatSection: false
title: "User Studies"
---

# User Studies

Security and privacy research often involves people directly. This includes interviews, surveys, lab studies, diary studies, usability tests, deception studies, and studies where participants install software, or interact with a prototype. Research can also involve people indirectly when it analyzes data derived from them, such as logs, posts, screenshots, telemetry, support tickets, browser histories, authentication data, or other behavioral traces. Involving people always creates ethical responsibilities. Researchers must treat participants and other affected people with respect, care, and transparency.

## Ethics Review

Research involving human participants or human-derived data should be reviewed by the appropriate institutional ethics review board, such as an IRB, ethics committee, or data protection office, where applicable. In some countries and institutional contexts, review is not optional: for example, in the United States, federally conducted or supported non-exempt human-subjects research is governed by the Common Rule, which includes requirements for IRB review and informed consent[^1]. If the study received approval, exemption, or a waiver, this should be disclosed in the paper.

However, institutional approval is neither always strictly necessary (some institutions even do not offer a review board) nor always sufficient to demonstrate ethical conduct. Some responsible studies may fall outside formal review requirements, while some formally approved studies may still raise ethical concerns. Authors should therefore reason about the ethics of their work beyond institutional compliance, explaining how they identified risks, protected participants and affected parties, and treated people with respect.

# Informed Consent

In most user studies, participants should be informed about the purpose of the study, what they will be asked to do, what data will be collected, how the data will be used, what risks may exist, and whether they can withdraw. Consent should be understandable, voluntary, and appropriate for the context.

Consent is especially important when studies involve sensitive topics, security behavior, privacy preferences, workplace practices, illegal or stigmatized behavior, marginalized groups, or vulnerable populations. Researchers should avoid consent forms that are technically complete but practically unreadable. Participants should understand the parts that matter for their decision.

An example consent form is offered by USENIX [here](https://www.usenix.org/sites/default/files/consent_author_proceedings.pdf).

## Deception

In most cases, participants should be fully informed about the purpose and risks of a study. Deception should be used only when it is necessary for the research question and when less deceptive alternatives would not work.

Security and privacy research sometimes uses deception, for example in phishing studies, or experiments about trust and decision-making. These studies can be valuable, but they also create risks: participants may feel embarrassed, manipulated, anxious, or less trusting after the study.

If deception is used, researchers should carefully justify why it is needed, minimize its scope, avoid unnecessary harm, and debrief participants afterward. The debriefing should explain what was concealed, why the deception was necessary, and how participants can ask questions or withdraw their data where feasible. Even mild deception should be treated as ethically relevant.

## What to Report in the Ethics Section

A paper involving user studies should include a clear ethics discussion. The section should state how participants were recruited, what they were told, how consent was obtained, what data was collected, and how the data was protected.

The ethics section should also discuss risks and mitigations. This includes risks to all stakeholders, the participants, bystanders, organizations, and affected communities. If the study involved PII or sensitive data, the paper should explain how harms were mitigated. If the study involved deception, the paper should justify why deception was necessary and describe the debriefing process.

## References
[^1]: https://www.ecfr.gov/current/title-45/subtitle-A/subchapter-A/part-46