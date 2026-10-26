# User Guide — Variable Group Comparison

## Free, read-only edition

This edition is free for all users, with no subscription or trial conversion. It cannot edit, propagate, delete or restore Variable Group data. The in-extension **User Guide** link opens this packaged document without requiring access to the private source repository.

## Comparison workspace

- Start with two palette colors; use **+** for up to five simultaneous comparison sets. Select at least two groups for each set, then run comparison.
- Browse Variable Groups in five-column, three-row pages using **<<** and **>>**. Hover a group to inspect its identifier.
- Type in **Search variable** to filter by key. Select Variable, Type or Status headers to change sort direction.
- Use the focus control beside search to expand results; use return or Escape to restore the layout. Collapse/expand palette and group sections when needed.
- Change language with the language selector. Saved selections are browser-local; current values are fetched again from Azure DevOps, not retained as a durable backup.
- Secret rows display **Manage from ADO Library**. Masked values do not prove that a secret is blank or equal across groups.

## Acknowledgement and support

After acceptance, the top notice shows terms version and acknowledgement time in this browser, with EULA/Privacy links. It is not identity-verified consent evidence. Cleared storage, another browser or changed terms can require acknowledgement again. Decline exits before the workspace starts.

Feedback offers a local email app, webmail or copy/download options; nothing sends email automatically. Opening webmail can transmit draft text to its provider before Send. Never include tokens, secrets or configuration values. Report download remains disabled in this candidate; Backup remains available.

## Security architecture disclosure — 14 October 2026

Comparison requests `vso.variablegroups_read` and performs no Variable Group writes. Read-only access still exposes accessible non-secret configuration; protect local exports and verify potentially stale results.

The current web package processes data in the user's browser and calls Azure DevOps through SDK authorization; it has no publisher-operated variable-data backend or automatic telemetry. Installation does not put it inside the customer's private network, and firewall/F5 protection is configuration-dependent. Local exports and user-selected email/documentation services are separate data boundaries. Marketplace scanning, iframe isolation and approved scopes reduce risk but are not a security certification or zero-data-loss guarantee.

See the edition's [Security architecture, limitations and remaining checks](security.md) and [Microsoft extension safety guidance](https://learn.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops#safety-information). Policy wording describes the current implementation, not a promise about unreviewed future releases.

> Offered free by an independent developer based in India, to help developers with everyday work. Thoroughly test the exact version in development or another lower/non-production environment before production use. Use production only after you are confident, have organizational approval, and have verified independent backup/recovery arrangements. You control your data and must verify results. The Publisher provides no managed data backup or guaranteed recovery; EULA limitations apply only where lawful.

1. Install the extension after reviewing its permission, EULA, and Privacy Policy.
2. Open a project and select **Pipelines > Variable Group Comparison**.
3. Accept the first-use terms and risk acknowledgement, or decline to exit.
4. Select one color and at least two Variable Groups, then choose **Run comparison**.
5. Search or sort the result and independently verify important findings in **Pipelines > Library**.
6. Select **Backup** at any time, choose any one or multiple accessible Variable Groups, and select **Download selected backup**. Store the downloaded CSV and matching manifest securely; secret values are excluded.
7. To inspect an earlier backup, open **Backup**, select **Preview restore**, choose the matching files, select one or multiple groups contained in the backup, and review the local dry-run. This edition cannot change Azure DevOps data.

Secret contents are never available to the extension. Manage them through Azure DevOps Library.
