# Support Policy — Variable Manager

## Security architecture disclosure — 14 October 2026

Editor requests `vso.variablegroups_manage` and can change authorized non-secret Variable Group values. Write access remains a material risk even if outbound traffic is blocked; use nonproduction testing and independent recovery.

The current web package processes data in the user's browser and calls Azure DevOps through SDK authorization; it has no publisher-operated variable-data backend or automatic telemetry. Installation does not put it inside the customer's private network, and firewall/F5 protection is configuration-dependent. Local exports and user-selected email/documentation services are separate data boundaries. Marketplace scanning, iframe isolation and approved scopes reduce risk but are not a security certification or zero-data-loss guarantee.

See the edition's [Security architecture, limitations and remaining checks](security.md) and [Microsoft extension safety guidance](https://learn.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops#safety-information). Policy wording describes the current implementation, not a promise about unreviewed future releases.

Document version: 2026-10-14; applies when supplied with a release.

## Independent developer support

An independent individual developer based in India provides this free extension to help other developers. Support is offered on reasonable efforts during available working time in India Standard Time, without an uptime, response, resolution, on-call, or data-recovery guarantee. This policy does not limit obligations imposed by applicable law.

Primary contact: adovgmanager@gmail.com. Marketplace Q&A is an additional route for non-confidential questions. The Feedback control prepares a draft or copyable message; it does not send email automatically. If a mail application does not open, copy the content or use the offered webmail or .eml fallback, review it, and send it yourself.

## Before production use

Thoroughly test the exact release in development or a lower/non-production environment first. Use representative fabricated data, test permissions and failure cases, and validate your independent backup/recovery arrangements. Use production only after you are confident and your organization approves. Re-test relevant workflows after upgrades.

## Reporting a problem

Include edition/version, browser/version, permission level, sanitized reproduction steps, expected/actual behavior, and redacted screenshots. Use fictional group names and values where possible. Organization/project names and group IDs are optional; provide them only if necessary and permitted by your organization. Never send passwords, PATs, access tokens, secret contents, confidential non-secret values, CSV backups, or unredacted reports.

For normal issues, the target acknowledgement is five business days, excluding Indian public holidays. Targets are not guarantees. Security and potentially incorrect-update reports receive priority; urgent incidents should also be handled through your organization's security/recovery process.

## Security reports

Email with subject SECURITY: Variable Manager. Describe the issue using fabricated data and minimal reproduction steps. Please report privately first so remediation can be coordinated. Do not send live credentials or customer datasets. The Publisher will investigate, coordinate necessary notices and fixes, and notify Microsoft about customer-impacting vulnerabilities as required by the applicable publisher agreement.

## Privacy and deletion

Email with subject PRIVACY REQUEST: Variable Manager. The Publisher will handle requests under applicable law and may need to verify the requester. Support email is handled through the Publisher's email provider as disclosed in the Privacy Policy. Clear browser site data to remove local preferences/acknowledgement.

## Service boundaries and retirement

Support does not provide production administration, guaranteed recovery, secret restoration, native Azure DevOps security changes, or support for Microsoft outages. Use your own approved recovery process. Contact Microsoft for Azure DevOps platform incidents.

The latest released version is the primary support target. Older versions may require upgrade after testing. If the Extension is retired, reasonable Marketplace notice will be provided where practicable, subject to urgent security/legal circumstances.
