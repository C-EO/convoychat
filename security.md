# ConvoyChat Security Vulnerability Disclosure Policy

**Last updated: January 18, 2023**

We, as the ConvoyChat Authors, take our responsibility to protect your data from unwarranted disclosure seriously. Equally we want security researchers to feel comfortable reporting security vulnerabilities they've discovered, as set out in this policy, so that we can fix them and keep your information safe.

This policy describes **what systems and types of research** are covered under this policy, **how to send us** vulnerability reports, and **how long** we ask security researchers to wait before publicly disclosing vulnerabilities.

## Guidelines

Before reporting any vulnerability, we require that you:

* Make every effort to avoid privacy violations, degradation of user experience, disruption to production systems, and destruction or manipulation of data.

* Only use exploits to the extent necessary to confirm a vulnerability. Do not use an exploit to compromise or exfiltrate data, establish command line access and/or persistence, or use the exploit to "pivot" to other systems. Once you've established that a vulnerability exists, or encountered any of the sensitive data outlined below, you must stop your test and notify us immediately.

* Keep confidential any information about discovered vulnerabilities for up to 90 calendar days after you have notified us. For details, please review **[Coordinated Disclosure](#coordinated-disclosure)**.

## Scope

> **Please note**: 
>
> This policy applies to the publicly available instance of ConvoyChat hosted at [https://convoychat.vercel.app](https://convoychat.vercel.app) only. 
>
> Any fix provided for the public instance will automatically apply to your instances.

The following test types are not authorized:

* UI/UX bugs or typos.
* Network denial of service (DoS or DDoS) tests.
* Physical testing (e.g. office access, open doors, tailgating) 
* Social engineering (e.g. phishing, vishing, etc.)
* Any other **non-technical** vulnerability testing.

If you encounter any of the below on our systems while testing within the scope of this policy, **[stop your test and notify us](#reporting-a-vulnerability)** immediately:

* Personally identifiable information (Commonly referred to as *Personal Information*)
* Financial information (e.g. credit card or bank account numbers)
* Proprietary information (e.g. trade secrets of a company or other entity)

## Authorization

If you make a good faith effort to comply with this policy during your security research, we will consider your research to be authorized, will work with you to understand and resolve the issue quickly, and we will not initiate or recommend legal action related to your research.

## Vulnerability Reporting

ConvoyChat does not currently have a *bug bounty programme*, but in an effort to support one in the future, we are working to set up our own instance of **[BugVilla](https://github.com/anuraghazra/bugvilla)**. 

In the meantime, we accept and discuss vulnerability reports via the [GitHub Security Tab](https://github.com/c-eo/convoychat/security).

A good vulnerability report should include:

* Description of the potential impact of the vulnerability.
* A detailed description of the steps required to reproduce the vulnerability. Proof of concept (POC) scripts, screenshots, and screen captures are all helpful. Please use extreme care to properly label and protect any exploit code.
* Any technical information and related materials we would need to reproduce the issue.

Please keep your vulnerability reports current by sending us any new information via [email](vulnerabilities.convoychat@gmail.com) as it becomes available.

Your email should include:

* An update label with the vulnerability title you used in the GitHub Security Tab.
* A link to the vulnerabilty report.
* An updated impact statement (Only if the impact level has changed.)
* Any new info you have concerning the vulnerability.
* Affected features of ConvoyChat.
* Your name, username and email address.
* A statement of good faith.
* A statement of your compliance to this policy.

You can copy and use the template below for your email:

```md
Update - Example Vulnerabilty

https://github.com/c-eo/convoychat/advisories/13

**Impact:** 1-3 - Low impact (Only if the impact level has changed.)

The **Example Vulnerability** causes an information leak to the room.

**Features Affected:** 

- Notification Component
- Invitation System

Dennis Sebalemba (C-EO) <dennis.sebalemba@gmail.com>

I have good faith that this security vulnerability will cause further more damage without this new information.

I agree to comply with the **[ConvoyChat Security Vulnerability Disclosure Policy](https://github.com/c-eo/convoychat/blob/main/docs/oss/security.md)**.
```

> The above template is in Markdown. In your email editor, please replace the Markdown with the RTF components provided. (e.g. `[Example](https://example.com)` will become link [Example](https://example.com).)

We may share your vulnerability reports with members of our community, as well as any affected vendors or open source projects.

## Coordinated Disclosure

We hope to patch vulnerabilities within 90 days or less, disclosing the details of those vulnerabilities when patches are published. We believe that public disclosure of vulnerabilities is an essential part of the vulnerability disclosure process, and that one of the best ways to make software better is to enable everyone to learn from each other's mistakes.

At the same time, we believe that disclosure in absence of a readily available patch tends to increase risk rather than reduce it, and so we ask that you refrain from sharing your report with others while we work on our patch. 

If you believe there are others that should be informed of your report before the patch is available, please let us know so we can make arrangements.

We may want to coordinate an advisory with you to be published simultaneously with the patch, but you are also welcome to self-disclose if you prefer. 

By default, we prefer to disclose everything, but we will never publish information about you or our communications with you without your permission. 

In some cases, we may also have some sensitive information that should be redacted, and so please check with us before self-disclosing.

## Conclusion

Thank you for taking time to read through this security vulnerability policy.

We hope to fix many vulnerabilities with you.
