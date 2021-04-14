---
external help file:
Module Name: Microsoft.Graph.Users.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.users.actions/add-mguserinsightsharedlastsharedmethodmicrosoftgraphworkbookrange
schema: 2.0.0
---

# Add-MgUserInsightSharedLastSharedMethodMicrosoftGraphWorkbookRange

## SYNOPSIS
Invoke action insert

## SYNTAX

### InsertExpanded (Default)
```
Add-MgUserInsightSharedLastSharedMethodMicrosoftGraphWorkbookRange -SharedInsightId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-Shift <String>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### Insert
```
Add-MgUserInsightSharedLastSharedMethodMicrosoftGraphWorkbookRange -SharedInsightId <String> -UserId <String>
 -BodyParameter <IPathsU4OqjcUsersUserIdInsightsSharedSharedinsightIdLastsharedmethodMicrosoftGraphWorkbookrangeMicrosoftGraphInsertPostRequestbodyContentApplicationJsonSchema>
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### InsertViaIdentity
```
Add-MgUserInsightSharedLastSharedMethodMicrosoftGraphWorkbookRange -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPathsU4OqjcUsersUserIdInsightsSharedSharedinsightIdLastsharedmethodMicrosoftGraphWorkbookrangeMicrosoftGraphInsertPostRequestbodyContentApplicationJsonSchema>
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### InsertViaIdentityExpanded
```
Add-MgUserInsightSharedLastSharedMethodMicrosoftGraphWorkbookRange -InputObject <IUsersActionsIdentity>
 [-AdditionalProperties <Hashtable>] [-Shift <String>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Invoke action insert

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: System.Collections.Hashtable
Parameter Sets: InsertExpanded, InsertViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IPathsU4OqjcUsersUserIdInsightsSharedSharedinsightIdLastsharedmethodMicrosoftGraphWorkbookrangeMicrosoftGraphInsertPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Insert, InsertViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
Parameter Sets: InsertViaIdentity, InsertViaIdentityExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SharedInsightId
key: id of sharedInsight

```yaml
Type: System.String
Parameter Sets: Insert, InsertExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Shift
.

```yaml
Type: System.String
Parameter Sets: InsertExpanded, InsertViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
key: id of user

```yaml
Type: System.String
Parameter Sets: Insert, InsertExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPathsU4OqjcUsersUserIdInsightsSharedSharedinsightIdLastsharedmethodMicrosoftGraphWorkbookrangeMicrosoftGraphInsertPostRequestbodyContentApplicationJsonSchema

### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity

## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphWorkbookRange

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IPathsU4OqjcUsersUserIdInsightsSharedSharedinsightIdLastsharedmethodMicrosoftGraphWorkbookrangeMicrosoftGraphInsertPostRequestbodyContentApplicationJsonSchema>: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Shift <String>]`: 

INPUTOBJECT <IUsersActionsIdentity>: Identity Parameter
  - `[AccessReviewInstanceId <String>]`: key: id of accessReviewInstance
  - `[AppLogCollectionRequestId <String>]`: key: id of appLogCollectionRequest
  - `[AuthenticationMethodId <String>]`: key: id of authenticationMethod
  - `[CalendarId <String>]`: key: id of calendar
  - `[DeviceEnrollmentConfigurationId <String>]`: key: id of deviceEnrollmentConfiguration
  - `[DeviceLogCollectionResponseId <String>]`: key: id of deviceLogCollectionResponse
  - `[EventId <String>]`: key: id of event
  - `[EventId1 <String>]`: key: id of event
  - `[MailFolderId <String>]`: key: id of mailFolder
  - `[MailFolderId1 <String>]`: key: id of mailFolder
  - `[ManagedDeviceId <String>]`: key: id of managedDevice
  - `[MessageId <String>]`: key: id of message
  - `[MobileAppTroubleshootingEventId <String>]`: key: id of mobileAppTroubleshootingEvent
  - `[NotebookId <String>]`: key: id of notebook
  - `[OnenotePageId <String>]`: key: id of onenotePage
  - `[OnenoteSectionId <String>]`: key: id of onenoteSection
  - `[OutlookTaskFolderId <String>]`: key: id of outlookTaskFolder
  - `[OutlookTaskGroupId <String>]`: key: id of outlookTaskGroup
  - `[OutlookTaskId <String>]`: key: id of outlookTask
  - `[SharedInsightId <String>]`: key: id of sharedInsight
  - `[TrendingId <String>]`: key: id of trending
  - `[UsedInsightId <String>]`: key: id of usedInsight
  - `[UserId <String>]`: key: id of user

## RELATED LINKS
