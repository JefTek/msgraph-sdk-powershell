<!-- region Generated -->
# Microsoft.Graph.Admin.WindowsUpdates
This directory contains the PowerShell module for the AdminWindowsUpdates service.

---
## Status
[![Microsoft.Graph.Admin.WindowsUpdates](https://img.shields.io/powershellgallery/v/Microsoft.Graph.Admin.WindowsUpdates.svg?style=flat-square&label=Microsoft.Graph.Admin.WindowsUpdates "Microsoft.Graph.Admin.WindowsUpdates")](https://www.powershellgallery.com/packages/Microsoft.Graph.Admin.WindowsUpdates/)

## Info
- Modifiable: yes
- Generated: all
- Committed: yes
- Packaged: yes

---
## Detail
This module was primarily generated via [AutoRest](https://github.com/Azure/autorest) using the [PowerShell](https://github.com/Azure/autorest.powershell) extension.

## Development
For information on how to develop for `Microsoft.Graph.Admin.WindowsUpdates`, see [how-to.md](how-to.md).
<!-- endregion -->

### AutoRest Configuration

> see https://aka.ms/autorest

``` yaml
require:
  - $(this-folder)/../../readme.graph.md
  - $(this-folder)/../../../profiles/$(title)/readme.md
title: $(service-name)
subject-prefix: ''
```

### Directives

> see https://github.com/Azure/autorest/blob/master/docs/powershell/directives.md

``` yaml
directive:
# Remove invalid paths.
  - remove-path-by-operation: ^admin(_.*Windows|.windows_.*Updates|.windows.updates.deployments_.*Audience)$
# Pluralize.
  - where:
      subject: (.*)WindowUpdate(.*)
    set:
      subject: $1WindowsUpdates$2
# Rename cmdlets.
  - where:
      verb: Add
      subject: ^(AdminWindowsUpdates)(DeploymentAudienceExclusion|DeploymentAudience|UpdatableAsset)(Member)$
      variant: ^Add1$|^AddExpanded1$|^AddViaIdentity1$|^AddViaIdentityExpanded1$
    set:
      subject: $1$2$3ById
  - where:
      verb: Remove
      subject: ^(AdminWindowsUpdates)(DeploymentAudienceExclusion|DeploymentAudience|UpdatableAsset)(Member)$
      variant: ^Remove1$|^RemoveExpanded1$|^RemoveViaIdentity1$|^RemoveViaIdentityExpanded1$
    set:
      subject: $1$2$3ById
  - where:
      verb: Invoke
      subject: ^(EnrollAdminWindowsUpdates)(DeploymentAudienceExclusion|DeploymentAudienceMember|Updatable)(Asset)$
      variant: ^Enroll1$|^EnrollExpanded1$|^EnrollViaIdentity1$|^EnrollViaIdentityExpanded1$
    set:
      subject: $1$2$3ById
  - where:
      verb: Invoke
      subject: ^(UnenrollAdminWindowsUpdates)(DeploymentAudienceExclusion|DeploymentAudienceMember|Updatable)(Asset)$
      variant: ^Unenroll1$|^UnenrollExpanded1$|^UnenrollViaIdentity1$|^UnenrollViaIdentityExpanded1$
    set:
      subject: $1$2$3ById
  - where:
      verb: Update
      subject: ^(AdminWindowsUpdatesDeploymentAudience)$
      variant: ^Update1$|^UpdateExpanded1$|^UpdateViaIdentity1$|^UpdateViaIdentityExpanded1$
    set:
      subject: $1ById
# Alias cmdlets.
# NB: We have to rename the command to the desired alias name, alias based on the rename, then undo the rename due to:
# - https://github.com/Azure/autorest.powershell/issues/769
  - where:
      subject: (.*)(AdminWindowsUpdates)(.*)
    set:
      subject: $1WU$3
      alias: ${verb}-Mg${subject}
  - where:
      subject: (.*)(WU)(.*)
    set:
      subject: $1AdminWindowsUpdates$3
```

### Versioning

``` yaml
module-version: 1.5.1
release-notes: See https://aka.ms/GraphPowerShell-Release.
```
