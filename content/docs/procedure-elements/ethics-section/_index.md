---
weight: 1
bookFlatSection: false
title: "Ethical Considerations Section"
---

# Ethical Considerations Section

An *Ethical Considerations* section is a specific section in a research paper to describe how the authors considered and addressed the ethical implications of their work. Its purpose is to make potential risks, harms, and broader societal impacts transparent to reviewers and readers, including future researchers.

A starting point suggested by USENIX and the Menlo Report is the *Stakeholder-Based Ethics Analysis*, including stakeholders and external systems involved in the research and considering their potential for harm (e.g., privacy risks) and benefit. It also explains how these risks were mitigated. Authors may also describe any approvals obtained (e.g., from an ethics board), as well as limitations of their approach and remaining concerns.

Importantly, this section should go beyond formal compliance. Even when no ethics approval is required, researchers are expected to reflect on the consequences of their methods and findings, and to justify why the work is ethically acceptable. Often a good ethics considerations section can already clarify questions that reviewers would have asked anyway.

## Stakeholder-Based Ethics Analysis

A stakeholder-based ethics analysis is a structured evaluation of how a research project and its publication may affect all relevant stakeholders such as participants, researchers, companies, and society both now and in the future. It identifies potential benefits and harms, explains mitigations, and justifies whether to proceed using ethical principles.

The following explanation is taken from [USENIX Security 2026](https://www.usenix.org/conference/usenixsecurity26/call-for-papers#ethics):

### Stakeholders
You are expected to consider all possible stakeholders (people, including the research team and society at large, and entities including companies) that may be impacted by your research. You are expected to detail how each stakeholder may have been impacted by the research procedures you undertook and how those stakeholders may be impacted by the publication of your research now and in the future.

### Impacts
* **Ethical principles**: You are expected to articulate the ethical principles you considered. A starting point is considering the principles in The Menlo Report in the context of each identified stakeholder: "Beneficence", "Respect for Persons", "Justice", and "Respect for Law and Public Interest".
* **Harms**: There are at least two broad categories of potentially negative outcomes from the research and publication process: tangible harms (e.g., financial loss or exposure to psychologically disturbing content) and violations of human rights even if there are no directly tangible harms (e.g., the violation of a participants' right to informed consent or the violation of users' right to privacy via the study of data that users expect and desire to be private).

### Mitigations
You are expected to detail both mitigated and unmitigated (potential) harms of your work. You are expected to detail the steps taken to mitigate harms.

### Decision
You are expected to articulate why the decision to proceed with the research and the decision to publish the research was reached, respectively. One approach to reaching such a decision is to weigh ethical harms against ethical benefits; see the "Beneficence" principle in The Menlo Report and the 2023 USENIX Security paper, "Ethical Frameworks and Computer Security Trolley Problems." An alternative or additional approach is to focus on avoiding the violation of individuals' rights; see the "Respect for Persons" principle in The Menlo Report and the discussion of deontological ethics in the above-cited 2023 USENIX Security paper.
* In some cases, the use of different principles in reaching an ethics decision will lead to the same conclusion for what is "right", e.g., the "Beneficence" and "Respect for Persons" analyses would agree. In other cases, the analyses may lead to different conclusions. If multiple analyses lead to the same conclusions, then documenting all those analyses will provide greater confidence in the ethics of the research. If different analyses lead to different conclusions on the ethics of the research, then the authors should clearly articulate how and why they chose the path they did, even if some principles would have led to a different decision. In some cases, researchers may need to make assumptions about the likelihood of different outcomes or the likely impacts of different decisions; in such cases, the authors are encouraged to articulate and justify all assumptions they make.
* When considering ethics, researchers and reviewers must acknowledge that, sometimes, the most ethical path is not to do the research or not to publish the research after it is complete.

## Why do I need it in my paper?

The PC Chairs of USENIX Security '26 wrote a [post](https://docs.google.com/document/d/e/2PACX-1vTBAZ4XrPejBY6EhPYhkXAS9l0pd9Qsl2HPbW26LJJOGp7gSGeWnd1mdoTC8kZuL95PvajiU4oBS4Ew/pub) on why they believe all papers should have an ethical considerations section.

## Examples

The following table lists a selection of papers we recommend as starting points for examples of well-developed ethics consideration sections.

Crypto:
* Li et al. [Shred-to-Shine Metamorphosis of (Distributed) Polynomial Commitments](https://www.usenix.org/sites/default/files/sec26cycle1-li-example.pdf). IACR.  2025

Machine Learning:
* Gong et al. [From Easy to Hard++: Promoting Differentially Private Image Synthesis Through Spatial-Frequency Curriculum](https://www.usenix.org/sites/default/files/conference-files/sec26cycle1-final514.pdf). USENIX. 2026

Network and Web:
* Chehade et al. [403 Forbidden? Ethically Evaluating Broken Access Control in the Wild](https://doi.ieeecomputersociety.org/10.1109/SP61157.2025.00252). SP. 2025
* Pan et al. [TORCHLIGHT: Shedding LIGHT on Real-World Attacks on Cloudless IoT Devices Concealed within the Tor Network](https://www.usenix.org/conference/usenixsecurity25/presentation/pan-yumingzhi). USENIX Security. 2025
* Heimbach et al. [Deanonymizing Ethereum Validators: The P2P Network Has a Privacy Issue](https://www.usenix.org/conference/usenixsecurity25/presentation/heimbach). USENIX Security. 2025
* Mustafa et al. [LEAKYLINKS: Measuring the Security and Privacy Risks of URL Scanning Services](https://swag.cispa.saarland/papers/mustafa2026leakylinks.pdf). SP. 2026

Software Security:
* Gong et al. [PAPILLON: Efficient and Stealthy Fuzz Testing-Powered Jailbreaks for LLMs](https://www.usenix.org/conference/usenixsecurity25/presentation/gong-xueluan). USENIX Security. 2025

Human Factors:
* Han et al. [Characterizing the MrDeepFakes Sexual Deepfake Marketplace](https://www.usenix.org/system/files/usenixsecurity25-han.pdf). USENIX Security. 2025
* Mukherjee et al. [Shadowed Realities: An Investigation of UI Attacks in WebXR](https://www.usenix.org/conference/usenixsecurity25/presentation/mukherjee). USENIX Security. 2025

ML & AI Security:
* Zhang et al. [Low-Cost and Comprehensive Non-textual Input Fuzzing with LLM-Synthesized Input Generators](https://www.usenix.org/conference/usenixsecurity25/presentation/zhang-kunpeng). USENIX Security. 2025