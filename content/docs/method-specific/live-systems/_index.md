---
weight: 1000
bookFlatSection: false
title: "Live Systems"
---

# Live Systems

Security and privacy research often studies live systems: websites, servers, APIs, network services, applications, or other infrastructure that is actively operated by someone else and used by real users. Such studies can be important because they reveal the prevalence of vulnerabilities, ecosystem-wide trends, misconfigurations, or privacy risks that cannot be fully understood in a lab environment. At the same time, interacting with live systems create an ethical challenge because the research activity itself may affect real people, organizations, and infrastructure [^1].

## Ethical Challenges to Consider

Live systems can fail, degrade, or behave unexpectedly. Even a small increase in resource usage may cause harm in unfavorable circumstances, for example if the target system is fragile, overloaded, rate-limited, poorly maintained, or used in a safety- or time-critical context like stock trading or medical context. Potential harms that researchers should consider include:

* disrupting normal system operation
* consuming any kind of resources (e.g., bandwidth, support staff)
* triggering alarms or abuse processes
* accessing or exposing confidential information
* modifying or overwriting data
* increasing risks for users if vulnerabilities are revealed or triggered (even just in log data for employees)

## Consent

In an ideal case, researchers have permission to interact with the systems they study. In practice, this is often not possible. For example, a study may analyze a broad trend across the Web, measure many independently operated systems, or crawl information from large organizations where requesting permission would be infeasible or would introduce major bias. In some cases, asking for consent from every affected operator would make the research impossible.

However, infeasibility of permission does not remove the responsibility to minimize harm. If researchers proceed without permission, they should be able to explain:

* why permission was not obtained
* why the study could not reasonably be conducted only in a lab study
* why the expected benefits justify interacting with live systems
* what steps were taken to reduce risk
* how operators or affected parties can contact the researchers (e.g., contact information in requests or an information page present when visiting the crawler IP)
* what the researchers plan to do in case harm, complaints, or unexpected effects occur

## Mitigation Strategies

Researchers should design live-system scans to be as conservative and non-disruptive as possible. Also, researchers can add some mitigations to minimize potential form harm (see [^2] and [^3]). These mitigations include:

* limiting the number of requests per host, network, organization, or time period
* avoiding repeated scans unless necessary
* testing the scanner on controlled systems before scanning live targets
* collecting only the data needed to answer the research question
* avoiding payloads that modify state, create accounts, submit forms, send messages, or write data
* monitor the scans and stop immediately when unexpected behavior or harm is observed
* providing a clear project webpage on the IP from which the scans originate
* Add contact address in a header or the user agent string of your requests
* offer and respecting opt-out requests
* [coordinating disclosure]({{< relref "docs/method-specific/live-systems/" >}}) if vulnerabilities are discovered

## Alternative Methods
When designing a scan on live systems, researchers should consider whether less intrusive alternatives are available. For example, when a study involves vulnerability testing, researchers should distinguish between confirming the existence of a vulnerability and exploiting it. In many cases, the former can be done with substantially less risk than the latter. Also, researchers should look into using existing datasets, conducting lab experiments, collaborating with operators, studying systems through vulnerability disclosure or bug bounty programs.

Bug bounty and vulnerability disclosure platforms can offer a useful alternative or complement because they provide clearer authorization boundaries and established communication channels. However, they may also introduce sampling bias, since participating organizations are not necessarily representative of the broader ecosystem (more on this in[^4]).

## Example Papers

* Chehade et al. [403 Forbidden? Ethically Evaluating Broken Access Control in the Wild](https://doi.ieeecomputersociety.org/10.1109/SP61157.2025.00252). SP. 2025
* Mustafa et al. [LEAKYLINKS: Measuring the Security and Privacy Risks of URL Scanning Services](https://swag.cispa.saarland/papers/mustafa2026leakylinks.pdf). SP. 2026

## References
[^1]: Partridge et al. [Ethical considerations in network measurement papers](https://dl.acm.org/doi/10.1145/2896816) Communications of the ACM. 2016.
[^2]: Hantke et al. [Where Are the Red Lines? Towards Ethical Server-Side Scans in Security and Privacy Research](https://doi.org/10.1109/SP54263.2024.00104). S&P. 2024.
[^3] Durumeric et al. [ZMap: Fast Internet-wide Scanning and Its Security Applications](https://www.usenix.org/system/files/conference/usenixsecurity13/sec13-paper_durumeric.pdf). USENIX. 2013.
[^4]: Decker et al. [VDPCollect: Vulnerability Disclosure Programs as a Complement to Web Security Measurements](https://swag.cispa.saarland/papers/decker2026vdpcollect.pdf). AsiaCCS. 2026.