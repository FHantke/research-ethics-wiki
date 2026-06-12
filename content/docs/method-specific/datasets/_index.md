---
weight: 1000
bookFlatSection: false
title: "Datasets"
---

# Datasets
Security and privacy research often relies on datasets collected by others. These datasets can be extremely valuable, especially when they provide insight into real-world attacks, user behavior, vulnerabilities, abuse ecosystems, or failures of deployed systems. However, some of these datasets were obtained through questionable, unauthorized, or illegal means like password leakage datasets or exposed server logs. This aspect has led to discussion within the community (see [^1] and [^2]).

## Publicly Available Does Not Mean Ethically Public

A common argument is that a dataset is acceptable to use because it is *already public*. This is not sufficient. Data may be technically accessible while still being private, sensitive, or published against the wishes and expectations of the people affected.

For example, a password dump posted online may be easy to download, but the affected users did not consent to their passwords being exposed or studied. Similarly, leaked emails, private messages, or account records may remain sensitive even if they are circulating publicly. Researchers should therefore distinguish between:

* data that was intentionally made public
* data that was accidentally exposed
* data that was stolen or leaked

The more questionable the origin of the dataset, the stronger the ethical justification and safeguards need to be.

## When Use May Be Justifiable

Using a questionable dataset is not automatically unethical, but it requires careful justification. A study may be more acceptable when:

* the research question is important and cannot reasonably be answered with safer data
* the dataset is uniquely valuable for understanding or reducing real-world harm
* the researchers took careful safeguards to secure the dataset
* the researchers did not participate in or encourage the original wrongdoing
* the work does not create new victims or substantially increase risk to existing victims
* the data is processed in a minimized, secure, and privacy-preserving way
* raw sensitive data is not redistributed
* the results are reported at an appropriate level of aggregation
* legal and institutional review has been considered
* the paper clearly explains the ethical reasoning

Weak justifications include: "others have used it before", "attackers already have it", "it was easy to find", or "it is technically public". These arguments may be relevant to the risk analysis, but they are not enough on their own.

## Questions to Ask Before Using a Dataset

Before using a dataset, researchers should ask:

* **Origin**: How was the dataset obtained? Was it collected with consent, leaked, stolen, scraped, purchased, or exposed by accident?
* **Legality**: Could downloading, storing, processing, or sharing the dataset violate laws, contracts, terms of service, or institutional rules?
* **Sensitivity**: Does the dataset contain passwords, tokens, private messages, financial data, health data, sexual content, political views, location traces, children’s data, or other sensitive information?
* **Identifiability**: Can individuals or organizations be identified directly or through linkage with other data?
* **Necessity**: Is this dataset necessary, or could the research question be answered with synthetic data, aggregated data, consented data, public documentation, or a less sensitive source?
* **Benefit**: What concrete scientific, security, privacy, or societal benefit does the study provide?
* **Harm**: What is the worst plausible harm if the dataset, code, model, or derived results are misused?
* **Safeguards**: How will access, storage, processing, deletion, and sharing be controlled?
* **Publication**: Could the paper help attackers find, reconstruct, validate, or exploit the data?

## Safeguards

Appropriate safeguards depend on the dataset and the research question, but may include:

* avoiding download of raw illegal data where possible
* storing data encrypted and access-controlled
* limiting access to approved project members
* keeping an access log
* replacing raw values with hashes if feasible
* avoiding publication of example records from real people
* publishing only aggregate statistics
* using synthetic examples in the paper and artifact
* not linking to, naming, or making the leaked dataset easier to find
* deleting the data after the project when retention is no longer justified
* documenting the data lifecycle in the ethics section


## What to Report in the Ethics Section

Papers using sensitive, leaked, hacked, or otherwise questionable datasets should include a dedicated ethics discussion. This section should explain:

* **Dataset origin**: What is known about how the dataset was created, leaked, exposed, or obtained?
* **Permission and consent**: Was consent or permission obtained? If not, why was this infeasible, and how were affected people’s interests protected?
* **Legal and institutional review**: Was an IRB, ethics board, legal office, data protection officer, or equivalent body consulted? If not, why not?
* **Necessity**: Why was this dataset needed, and what alternatives were considered?
* **Risks**: What harms could arise from possession, analysis, publication, or artifact release?
* **Benefits**: What concrete benefits justify the use of the dataset?
* **Safeguards**: How was the data stored, minimized, transformed, protected, and eventually deleted?

The goal is to show that the researchers understood the origin and sensitivity of the data, considered the people and organizations affected, weighed harms against benefits, and chose safeguards appropriate to the risk.

## References
[^1]: Egelman et al. [It's Not Stealing If You Need It: A Panel on the Ethics of Performing Research Using Public Data of Illicit Origin](https://doi.org/10.1007/978-3-642-34638-5_11). Workshop on Ethics in Computer Security Research. 2012. 
[^2]: Thomas et al. [Ethical Issues in Research Using Datasets of Illicit Origin](https://dl.acm.org/doi/abs/10.1145/3131365.3131389). IMC. 2017.