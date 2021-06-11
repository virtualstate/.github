# Security Policy

This document describes the management of vulnerabilities for the
Virtual State project and its official plugins.

## Reporting vulnerabilities

Please contact [vulnerabilities@axiom.contact](mailto:vulnerabilities@axiom.contact) 

## Handling vulnerability reports

When a potential vulnerability is reported, the following actions are taken:

### Triage

**Delay:** 4 business days

Within 4 business days, a member of the team provides a first answer to the
individual who submitted the potential vulnerability. The possible responses
can be:

* Acceptance: what was reported is considered as a new vulnerability
* Rejection: what was reported is not considered as a new vulnerability
* Need more information: the team needs more information in order to evaluate what was reported.

Triaging should include updating issue fields:
* Asset - set/create the module affected by the report
* Severity - TBD, currently left empty

### Correction follow-up

**Delay:** 90 days

When a vulnerability is confirmed, a member of the team volunteers to follow
up on this report.

With the help of the individual who reported the vulnerability, they contact
the maintainers of the vulnerable package to make them aware of the
vulnerability. The maintainers can be invited as participants to the reported issue.

With the package maintainer, they define a release date for the publication
of the vulnerability. Ideally, this release date should not happen before
the package has been patched.

The report's vulnerable versions upper limit should be set to:
* `*` if there is no fixed version available by the time of publishing the report.
* the last vulnerable version. For example: `<=1.2.3` if a fix exists in `1.2.4`

### Publication

**Delay:** 90 days

Within 90 days after the triage date, the vulnerability must be made public.

**Severity**: Vulnerability severity is assessed using [CVSS v.3](https://www.first.org/cvss/user-guide).
More information can be found on [HackerOne documentation](https://docs.hackerone.com/hackers/severity.html)

If the package maintainer is actively developing a patch, an additional delay
can be added with the approval of the security team and the individual who
reported the vulnerability. 

At this point, a CVE should be requested through the HackerOne platform through
the UI, which should include the Report ID and a summary.

## The team

The core team is responsible for the management of this policy and process.

Members of this team are expected to keep all information that they have privileged access to by being
on the team completely private to the team. This includes agreeing to not notify anyone outside the
team of issues that have not yet been disclosed publicly, including the existence of issues,
expectations of upcoming releases, and patching of any issues other than in the process of their work
as a member of the Virtual State Core team.

### Members

* [__Fabian Cook__](https://github.com/fabiancook), <https://twitter.com/fabiancook>
