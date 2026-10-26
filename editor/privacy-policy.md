# Privacy Policy — Variable Manager

## Security architecture disclosure — 14 October 2026

Editor requests `vso.variablegroups_manage` and can change authorized non-secret Variable Group values. Write access remains a material risk even if outbound traffic is blocked; use nonproduction testing and independent recovery. Feedback webmail compose URLs can disclose the selected draft text to the provider before Send. Documentation hosts receive normal browser/network metadata. Therefore 'no publisher-hosted variable-data backend' does not mean 'no external browser traffic'.

The current web package processes data in the user's browser and calls Azure DevOps through SDK authorization; it has no publisher-operated variable-data backend or automatic telemetry. Installation does not put it inside the customer's private network, and firewall/F5 protection is configuration-dependent. Local exports and user-selected email/documentation services are separate data boundaries. Marketplace scanning, iframe isolation and approved scopes reduce risk but are not a security certification or zero-data-loss guarantee.

See the edition's [Security architecture, limitations and remaining checks](security.md) and [Microsoft extension safety guidance](https://learn.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops#safety-information). Policy wording describes the current implementation, not a promise about unreviewed future releases.

Document version: 2026-10-25; applies when supplied with a release.

The top-page acknowledgement notice reads the existing browser-local terms version and acceptance timestamp. It adds no user identity, IP address or publisher-side consent record. If storage is blocked, the notice uses memory for that page session only. This is not a verified per-user acceptance ledger.

## Data processing

Variable-group identifiers, names, keys, types, and non-secret values are processed in the user’s browser. Confirmed edits are sent directly to Azure DevOps.

The current shipped configuration has no publisher-operated telemetry, analytics, advertising, storage, licensing, or approval endpoint. Its Variable Group workflow does not automatically send configuration data to a publisher service. UI preferences, selected group metadata where applicable, and legal acknowledgement are stored in browser local storage for the extension origin. Local exports, documentation visits and user-selected feedback services are separate boundaries described in this policy.

When the user requests a backup, the extension freshly reads only the Variable Groups selected in the independent Backup workspace and generates a CSV plus metadata manifest locally in the browser. A comparison is not required. Non-secret values are included, secret contents are excluded, and the files are downloaded without being sent to the Publisher. For restore, the user selects a matching CSV and manifest and then selects one or multiple groups contained in the backup. The files are validated in browser memory and are not uploaded or retained by the extension. Only after the user selects Restore and confirms can reviewed non-secret add/update values be written to Azure DevOps. A downloaded restore receipt contains operation metadata and outcomes, not variable values. The customer controls storage, retention, sharing, and deletion of downloaded files.

Secret values are not read or displayed. Azure DevOps may identify a secret variable without returning its value.

When the user selects Download Report, the extension creates an HTML report locally in the browser from the currently loaded comparison. It can contain Variable Group names, variable keys, and non-secret values. Secret contents are excluded. The report is downloaded to the user's device and is not sent to the Publisher; the customer controls its storage, retention, sharing, and deletion.

## Storage boundary

The current Editor does not write update records, actor identities, variable keys, values, or secret contents to Azure DevOps Extension Data or publisher-operated storage. UI preferences and acknowledgement remain browser-local; user-requested exports remain under the user's control.

## User-initiated feedback

Feedback lets the user choose a local email application, Gmail web, Outlook web, clipboard copy, or a locally downloaded `.eml` draft. No email is sent automatically. Gmail or Outlook is opened only when the user selects it; opening the compose URL can transmit the draft recipient, subject and body to that provider before Send is clicked. The user must sign in if necessary, review, and send the message. If sent, the email and anything the user adds are processed by the selected email provider and the Publisher's mailbox provider. Clipboard and downloaded files remain under the user’s control. Do not include secrets, credentials, tokens, or variable values.

## External services and future changes

The Extension is free and has no subscription or licensing service. This policy and the Extension disclosures must be revised before any external approval, analytics, storage, billing, or entitlement service is enabled.

## Retention and rights

The Publisher retains only support email that a user voluntarily sends, for as long as reasonably needed to respond, meet legal obligations, and protect against abuse. Applicable access, correction, or deletion requests may be sent to the contact below. Azure DevOps tenant data remains subject to the customer’s and Microsoft’s controls.

## Security and contact

Reasonable safeguards are used, but no system is risk-free. Report privacy questions or security concerns to adovgmanager@gmail.com. Provider: the publisher identified in the official Marketplace listing, an independent individual developer based in India.

## User control and testing

You retain ownership of your data and control Azure DevOps access and local exports. Test the exact extension release thoroughly in development or another lower/non-production environment before production use. The Publisher does not operate a managed backup or recovery service. This does not remove any statutory privacy or security obligations.

Support email may include your address, name, reproduction details, and voluntarily supplied metadata. It is processed by the Publisher and the selected email providers, including the Publisher's Gmail mailbox, to respond to requests, maintain security, and meet applicable legal obligations. It is not used for advertising or sale. Delete resolved correspondence when no longer reasonably needed; legal/security obligations may require longer retention. Requests for access, correction, or deletion can be sent to adovgmanager@gmail.com and will be handled subject to applicable law and necessary identity verification. External providers operate under their own policies; customer Azure DevOps data remains subject to customer and Microsoft controls.
