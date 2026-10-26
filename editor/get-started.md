# Getting Started with Variable Manager

## Security architecture disclosure — 14 October 2026

Editor requests `vso.variablegroups_manage` and can change authorized non-secret Variable Group values. Write access remains a material risk even if outbound traffic is blocked; use nonproduction testing and independent recovery.

The current web package processes data in the user's browser and calls Azure DevOps through SDK authorization; it has no publisher-operated variable-data backend or automatic telemetry. Installation does not put it inside the customer's private network, and firewall/F5 protection is configuration-dependent. Local exports and user-selected email/documentation services are separate data boundaries. Marketplace scanning, iframe isolation and approved scopes reduce risk but are not a security certification or zero-data-loss guarantee.

See the edition's [Security architecture, limitations and remaining checks](security.md) and [Microsoft extension safety guidance](https://learn.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops#safety-information). Policy wording describes the current implementation, not a promise about unreviewed future releases.

> Offered free by an independent developer based in India, to help developers with everyday work. Thoroughly test the exact version in development or another lower/non-production environment before production use. Use production only after you are confident, have organizational approval, and have verified independent backup/recovery arrangements. You control your data and must verify results and every proposed update. The Publisher provides no managed data backup or guaranteed recovery; EULA limitations apply only where lawful.

Document version: 24 September 2026; effective with the reviewed public release.

## Before installation

1. Read the EULA, Privacy Policy, and Support Policy.
2. Confirm that the installer is authorized to accept the terms for the organization.
3. Review the requested Azure DevOps scope.
4. Confirm that the organization has an independent change-control and recovery process.
5. Test the extension in a non-production project first.

## Install

1. Open the Variable Manager page in Visual Studio Marketplace and select **Get it free**.
2. Select the Azure DevOps organization and review the permissions and legal links.
3. Install the extension.
4. Open an Azure DevOps project and go to **Pipelines > Variable Manager**.
5. Accept the first-use terms/risk acknowledgement, or decline to exit without loading project data.

## Compare and update

1. Choose a palette color, select two or more Variable Groups, and select **Run comparison**.
2. Review matching, different, and missing values. Search or sort the rows, or use the target button beside Search variable to open the result in a full-page workspace. Use the return button or Escape to go back.
3. For a non-secret value, enter the new value and choose whether to propagate it.
4. Independently verify any resulting values in Azure DevOps Library.
5. Select **Download Report** to download a local HTML report of the loaded comparison results.

The signed-in user must have explicit Azure DevOps update permission for every affected Variable Group. Secret values remain managed through Azure DevOps Library.

## Backup and restore

1. Select **Backup** at any time; a comparison is not required.
2. Select any one or multiple accessible Variable Groups.
3. Select **Download selected backup** to generate a local CSV and matching manifest from fresh Azure DevOps state.
4. To recover data, open **Backup**, select **Restore**, choose the matching CSV and manifest, and select the group or groups contained in the backup that you want to preview.
5. Review the dry-run. If you continue, choose whether to take a fresh current-state backup, review the final warning, and confirm.

Restore applies only reviewed non-secret add/update differences. It fails closed on missing permission or concurrency conflicts, never deletes current-only variables, and downloads a value-free receipt. Backups exclude secret values and are not guaranteed rollback. Store backup files securely.

## Support

Use **Feedback** or email `adovgmanager@gmail.com`. Include the organization, project, Variable Group IDs, extension version, and reproduction steps. Do not include secrets or access tokens.
