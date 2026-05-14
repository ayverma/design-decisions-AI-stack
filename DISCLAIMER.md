# Scope, Third-Party Terms, and User Responsibility

> Read this once before using the contents of this repository in any setting that involves real accounting, financial, or personal data.

---

## 1. What this repository IS

A **behavior-specification framework** for AI assistants. It consists of:

- An interactive HTML document for capturing design decisions (sliders, approve/deny toggles, stack picks).
- A JSON-LD schema describing how AI assistants should behave at **inference time** (reading the spec → reasoning → producing output) when helping a user assemble reports, dashboards, or applications.
- A README explaining how non-technical users can adjust AI behavior by editing the spec.

The framework is **vendor-neutral**. Any data source, database, AI model, hosting service, or chatbot frontend named in the schema is provided as an **example or category placeholder**, not a recommendation, endorsement, or required dependency.

---

## 2. What this repository IS NOT

This repository **does not**:

- Process, store, transmit, retain, or transform any user data.
- Connect to any data source, API, OData feed, accounting platform, or third-party service.
- Train, fine-tune, adapt, distill, or enhance any AI or machine learning model.
- Generate prompts that, by their content, instruct an AI to train a model on third-party data.
- Ship credentials, tokens, or any form of access to a third-party system.
- Provide a hosted service, runtime, executable application, or SaaS endpoint.
- Constitute legal, financial, accounting, audit, or tax advice.

The artifacts in this repository are **specifications and documentation only**. They describe how AI assistants *could be configured* to behave; they do not themselves perform any action against external systems.

---

## 3. Third-Party Terms — User Responsibility

If you, as a user of this framework, connect an AI assistant to any third-party service — including but not limited to **Xero, MYOB, QuickBooks, OdataLink, Notion, Monday.com, Microsoft, Google, Amazon Web Services, Anthropic, OpenAI, any database vendor, or any hosting provider** — you alone are responsible for:

- Reading, understanding, and complying with that service's terms of service, developer terms, fair-use policy, data-processing addendum, and any applicable privacy or AI policy.
- Obtaining any consent required from data subjects, end users, or rights holders before retrieving, processing, or transmitting their data.
- Ensuring that your downstream use of the data — including any use of an AI model on that data — is permitted under the terms of the originating service.
- Bearing all costs, fees, rate-limit consequences, and contractual obligations that arise from your use of those services.

The maintainers of this repository have no agency, contract, or relationship with the providers of any third-party service referenced as an example in this framework, and accept no responsibility for your compliance with those providers' terms.

---

## 4. Specific Notice — Xero Developer Platform Terms (effective 2 March 2026)

Xero's revised Developer Platform Terms and Conditions, taking effect 2 March 2026, contain restrictions that include, among other things:

- A prohibition on using API Data to train, fine-tune, adapt, or enhance any AI or machine learning model.
- A prohibition on passing API Data to a third party without the associated user's consent.

If you obtain accounting data that originated from Xero — whether directly via Xero's API, indirectly via OdataLink's OData feeds, or via any other intermediary — those restrictions may apply to your use of that data.

**This repository does not facilitate, encourage, or enable AI model training on Xero-originated data, or on any third-party data.** The AI-behavior settings described in the framework concern *inference-time* reasoning (reading data and producing a report for the requesting user) and *short-lived contextual memory of user corrections* (stored locally for the requesting user's benefit only). Neither of these activities, as described in the framework, constitutes training a model.

You remain solely responsible for verifying that your specific configuration and downstream use of any AI assistant or memory store complies with all applicable third-party terms.

---

## 5. OdataLink Fair Use

If you use OdataLink to obtain OData feeds from a connected accounting system, OdataLink's [Fair Use Policy](https://odatalink.com/fair-use-policy) and [End User License Agreement](https://odatalink.com/eula) apply to your account, your data downloads, and any costs that arise from your usage patterns.

This repository does not consume, cache, replay, multiply, or otherwise affect OdataLink data downloads. The user — through the tools and configurations they choose to deploy based on this framework — is the party responsible for staying within their Monthly Download Allowance and for any custom-pricing arrangements that follow from excessive use.

---

## 6. Vendor and Tool Names — Examples Only

The framework lists various technology options in its stack matrix and example schemas (databases, dashboards, frontends, model providers, hosting platforms, and so on). Every such name is provided as a **category example** so that users understand the kinds of choices available to them. The presence of a name in this repository:

- is not an endorsement, certification, partnership, or recommendation;
- does not imply any commercial relationship between the repository's maintainers and the named vendor;
- does not imply that the named vendor has reviewed, approved, or is aware of this repository;
- and may change at any time without notice.

Users are free to substitute any equivalent or alternative service, and are encouraged to evaluate fit, cost, terms, and compliance on their own merits.

---

## 7. User Attestation

By using the configurations, prompts, schemas, or other artifacts derived from this repository in connection with any real data or any third-party service, you attest that:

- You have read and accepted the terms of every third-party service involved in your configuration.
- You have authority to use the data you intend to process.
- You will not use the framework, or any prompts derived from it, to train, fine-tune, or otherwise enhance any AI or machine learning model on data whose source terms prohibit such use.
- You understand that AI-generated output may contain errors, omissions, or fabrications, and that responsibility for verifying and acting on AI output rests with you.
- You will not represent any output produced via this framework as having been reviewed, certified, or endorsed by the repository's maintainers or by the providers of any third-party service named in the framework.

---

## 8. No Warranty; Limitation of Liability

The artifacts in this repository are provided "as is," without warranty of any kind, express or implied, including but not limited to warranties of merchantability, fitness for a particular purpose, accuracy, completeness, or non-infringement.

To the maximum extent permitted by applicable law, the maintainers and contributors shall not be liable for any direct, indirect, incidental, special, consequential, or punitive damages — including loss of profits, revenue, data, goodwill, or business — arising from or related to your use of this repository, even if advised of the possibility of such damages.

This limitation applies whether the alleged harm arises from breach of contract, tort, statute, or any other legal theory, and survives any termination of your use of the repository.

---

## 9. Changes to this Document

This disclaimer may be updated to reflect changes in third-party terms, applicable law, or the scope of the repository. The version effective at the time of your use is the version present in the `main` branch of the repository on the date of use. Material changes will be noted in the repository's commit history.

---

## 10. Governing Law

For matters concerning the maintainers' obligations and any disputes arising from the repository itself (as distinct from third-party services), the laws of the jurisdiction in which the maintainer entity is registered shall apply, without regard to conflict-of-laws principles. Disputes shall be resolved in the courts of that jurisdiction.

For matters concerning any third-party service you connect to, the governing law specified by that service's terms applies, and disputes are resolved under those terms.

---

_This disclaimer is provided for clarity of scope and is not a substitute for legal advice. If your intended use raises specific compliance questions, consult a qualified lawyer in your jurisdiction._

_Last reviewed: 2026-05-14_
