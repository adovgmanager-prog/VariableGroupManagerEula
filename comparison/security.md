# Security Reporting — Variable Group Comparison

## Architecture and security disclosure

Reviewed: 14 October 2026; current Azure DevOps Services web edition. This is source-based disclosure, not an independent security certification.

Comparison requests `vso.variablegroups_read` and performs no Variable Group writes. Read-only access still exposes accessible non-secret configuration; protect local exports and verify potentially stale results. See [Microsoft scope definitions](https://learn.microsoft.com/en-us/azure/devops/extend/develop/manifest?view=azure-devops#scopes).

The packaged interface runs in a browser iframe and uses Azure DevOps SDK authorization for the signed-in user. Native Azure DevOps permissions remain authoritative. Microsoft describes Marketplace virus/content scanning and approved scopes, but these do not prove the absence of defects or malicious behavior. See [Microsoft extension safety guidance](https://learn.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops#safety-information) and [Microsoft authentication guidance](https://learn.microsoft.com/en-us/azure/devops/extend/develop/auth?view=azure-devops).

Installation in a SaaS organization does not place the extension inside a private customer LAN/VNet. Firewall/F5 controls depend on actual routing and policies. The current hub CSP limits script and API connection sources but is not an absolute external-transmission guarantee.

The current package has no publisher-hosted customer-value database or automatic telemetry. Values are processed in browser memory. Preferences/selected group metadata and terms acknowledgement may be browser-local; local exports can contain non-secret values and remain the customer's responsibility. SDK tokens are used for authorization, not intentionally persisted in preferences or exports; no PAT/password input is required. Secret contents are excluded from comparison/edit/export/restore and managed in Azure DevOps Library.

Feedback may pass draft text to a selected webmail provider when its compose page opens, before Send. Public documentation links expose normal browser metadata to their hosts. Voluntary support correspondence is processed by email providers. Do not submit configuration values or credentials.

No publisher-operated backend is required for this edition's current Variable Group workflow.

### Missing evidence and release checks

Installed-package role/permission tests, network/storage/CSP verification, XSS/import regression coverage, refreshed dependency/SBOM review, anonymous public-document URLs and final Marketplace acceptance remain release checks; this documentation update does not complete them. No specific export-encryption algorithm, TLS version, legal compliance certification or independent penetration test is claimed. Test read-only boundaries and sensitive local-export handling.

[Microsoft high-privilege guidance](https://learn.microsoft.com/en-us/azure/devops/marketplace/manage-high-privilege-extensions?view=azure-devops) explains the need to assess scope necessity and publisher/code trust. Microsoft platform controls, publisher implementation duties and customer permissions/network/recovery duties are complementary, not a guarantee of security or immunity from liability.

For questions about security architecture, release evidence or outstanding validation, contact adovgmanager@gmail.com. This public page is self-contained; the private source repository and internal review records are not published here.

Report suspected vulnerabilities privately to adovgmanager@gmail.com. Include the edition, version, reproduction steps, and impact, but do not email secrets, credentials, tokens, personal data, or production variable values.

The Publisher will acknowledge reports as reasonably practicable, investigate, coordinate remediation, and communicate material release guidance. Do not publicly disclose an unremediated vulnerability before coordinated disclosure.

The extension uses Azure DevOps SDK APIs and the edition-specific scopes disclosed above. The current shipped configuration has no publisher-operated backend, analytics, or telemetry. Scope necessity and implied capabilities must be reassessed per release.
