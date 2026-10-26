# End User License Agreement — Variable Manager

## Security architecture disclosure — 14 October 2026

Editor requests `vso.variablegroups_manage` and can change authorized non-secret Variable Group values. Write access remains a material risk even if outbound traffic is blocked; use nonproduction testing and independent recovery. This explanatory security note does not grant new permissions, certify safety, replace organization approval, or override non-waivable legal obligations.

The current web package processes data in the user's browser and calls Azure DevOps through SDK authorization; it has no publisher-operated variable-data backend or automatic telemetry. Installation does not put it inside the customer's private network, and firewall/F5 protection is configuration-dependent. Local exports and user-selected email/documentation services are separate data boundaries. Marketplace scanning, iframe isolation and approved scopes reduce risk but are not a security certification or zero-data-loss guarantee.

See the edition's [Security architecture, limitations and remaining checks](security.md) and [Microsoft extension safety guidance](https://learn.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops#safety-information). Policy wording describes the current implementation, not a promise about unreviewed future releases.

Document version: 2026-10-25. Applies when supplied with a release; revised terms apply prospectively.

## Publisher and purpose

Variable Manager (the Extension) is offered by the publisher identified on this Extension's official Visual Studio Marketplace listing (the Publisher), an independent individual developer based in India, to help developers with everyday Azure DevOps work. The Marketplace listing identifies the contracting provider; omission of a personal name here does not make the provider anonymous or remove required identity disclosures. The Publisher is not Microsoft and does not offer a managed production service. Microsoft does not endorse this Extension. Contact: adovgmanager@gmail.com.

## Acceptance and permitted use

Read these terms before use. Selecting the in-product acceptance control indicates acceptance. If acting for an organization, you must have authority to accept these terms on its behalf; otherwise obtain that authority or decline and do not use the Extension.

The Publisher grants a non-exclusive, non-transferable licence to use the Extension for lawful internal personal or organizational work with Azure DevOps. The Extension remains proprietary; being free does not make it open source or grant ownership of its code. Third-party components remain subject to their own licences. Do not resell, sublicense, unlawfully redistribute, bypass access controls, or reverse engineer except where applicable law grants that right.

## Edition capabilities and limits

Bundled runtime copyright and licence texts are retained in [Third-Party Notices](third-party-notices.md). These upstream notices remain intact and are not removed by the request to omit the Publisher's personal name.

The Extension reads Variable Groups and permits authorized non-secret edits, propagation, and guarded add/update restore. Confirmed operations change original Azure DevOps data and can affect pipelines and applications. Restore can partially complete, does not delete current-only variables, and is not guaranteed rollback.

Azure DevOps controls native access permissions. Secret contents are unavailable to the Extension and must be managed through Azure DevOps Library. The Extension does not replace Azure DevOps security, organizational change approval, independent backup, disaster recovery, or compliance auditing.

## Free use

This Marketplace edition is free. No subscription, licence key, automatic trial conversion, or separate payment is required. A future paid Locked Azure Managed Application would be a separate product with separate terms and infrastructure charges; it does not convert this free extension into a paid product. Azure DevOps and other services may have their own charges.

## Your responsibility for data and production use

You retain ownership and control of your data. You and your organization are responsible for permissions, lawful processing, selection of the organization/project/groups, source and target values, verification of results, downloaded files, independent backups, recovery arrangements, and approval of production use.

**Thoroughly test the exact extension version in development or another lower/non-production environment with representative fabricated data before production use. Only use it in production after you are confident in its behavior, permissions, limitations, and your tested recovery procedures, and after obtaining organizational approval.** Repeat relevant testing after upgrades. No test eliminates all risk.

Before every edit, propagation, or restore, verify targets and preserve an independent recoverable copy of affected non-secret data. Maintain separate recovery arrangements for secrets, permissions, Key Vault links, and other content excluded from backups. Avoid simultaneous updates and verify the final state directly in Azure DevOps Library.

Never place passwords, tokens, secret contents, or confidential values in support messages or screenshots. Secure downloaded backups/reports; local exports can contain non-secret values and the Publisher does not retain or recover them for you.

## Warranty and recovery disclaimer

To the maximum extent permitted by applicable law, the Extension is provided **as is** and **as available**, without express or implied warranties, including accuracy, uninterrupted availability, merchantability, fitness for a particular purpose, or suitability for production. Bugs, stale data, concurrency conflicts, browser problems, service failures, and partial operations may occur.

The Publisher does not undertake to host, back up, restore, insure, or manage your Variable Group data or your production environment. Support is provided on reasonable efforts as described in the Support Policy, with no guaranteed uptime, response, resolution, or recovery commitment.

## Limitation of liability

To the maximum extent permitted by applicable law, the Publisher is not liable for loss, corruption, or unavailability of data, loss of profits or revenue, business interruption, or indirect, incidental, special, consequential, or punitive damages arising from use of or inability to use the Extension, including mistaken edits, source/target selection, stale comparisons, propagation, import/restore operations, missing backups, or reliance on results.

To the maximum extent permitted by applicable law, the Publisher's aggregate liability for other claims arising from the Extension is limited to USD 100. This is a contractual limit, not insurance or a recovery promise.

Nothing excludes or limits rights or liabilities that cannot lawfully be excluded or limited, including applicable statutory consumer rights or liability for fraud, wilful misconduct, or other conduct for which applicable law prohibits exclusion. These terms do not release the Publisher from mandatory privacy, security, intellectual-property, or other legal obligations. If a provision is unenforceable, it applies only to the extent lawful and the remaining provisions continue.

## Privacy, changes, and termination

Data handling is described in the Privacy Policy. Material changes are documented with a new terms version and presented for acknowledgement when delivered through the Extension. Changes do not retroactively waive existing rights. Stop using and uninstall the Extension if you do not accept revised terms.

The Publisher may end this licence for a material breach or discontinue the Extension with reasonable notice where practicable. Mandatory legal notice and rights remain applicable. Ownership, lawful limitations, and provisions intended to survive termination continue.

## Applicable law and contact

These terms are governed by the laws of India, subject to mandatory protections and jurisdiction rights applicable to you. No exclusive court venue is imposed by these terms. Questions, privacy requests, and support: adovgmanager@gmail.com.
