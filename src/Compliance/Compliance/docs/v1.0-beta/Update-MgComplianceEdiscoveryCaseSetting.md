---
external help file:
Module Name: Microsoft.Graph.Compliance
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.compliance/update-mgcomplianceediscoverycasesetting
schema: 2.0.0
---

# Update-MgComplianceEdiscoveryCaseSetting

## SYNOPSIS
Update the navigation property settings in compliance

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgComplianceEdiscoveryCaseSetting -CaseId <String> [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-Ocr <IMicrosoftGraphEdiscoveryOcrSettings>]
 [-RedundancyDetection <IMicrosoftGraphEdiscoveryRedundancyDetectionSettings>]
 [-TopicModeling <IMicrosoftGraphEdiscoveryTopicModelingSettings>] [-PassThru] [-Confirm] [-WhatIf]
 [<CommonParameters>]
```

### Update
```
Update-MgComplianceEdiscoveryCaseSetting -CaseId <String> -BodyParameter <IMicrosoftGraphEdiscoverySettings>
 [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgComplianceEdiscoveryCaseSetting -InputObject <IComplianceIdentity>
 -BodyParameter <IMicrosoftGraphEdiscoverySettings> [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgComplianceEdiscoveryCaseSetting -InputObject <IComplianceIdentity>
 [-AdditionalProperties <Hashtable>] [-Id <String>] [-Ocr <IMicrosoftGraphEdiscoveryOcrSettings>]
 [-RedundancyDetection <IMicrosoftGraphEdiscoveryRedundancyDetectionSettings>]
 [-TopicModeling <IMicrosoftGraphEdiscoveryTopicModelingSettings>] [-PassThru] [-Confirm] [-WhatIf]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property settings in compliance

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: System.Collections.Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
settings
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEdiscoverySettings
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CaseId
key: id of case

```yaml
Type: System.String
Parameter Sets: Update, UpdateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Read-only.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IComplianceIdentity
Parameter Sets: UpdateViaIdentity, UpdateViaIdentityExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Ocr
ocrSettings
To construct, see NOTES section for OCR properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEdiscoveryOcrSettings
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RedundancyDetection
redundancyDetectionSettings
To construct, see NOTES section for REDUNDANCYDETECTION properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEdiscoveryRedundancyDetectionSettings
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TopicModeling
topicModelingSettings
To construct, see NOTES section for TOPICMODELING properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEdiscoveryTopicModelingSettings
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
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

### Microsoft.Graph.PowerShell.Models.IComplianceIdentity

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEdiscoverySettings

## OUTPUTS

### System.Boolean

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IMicrosoftGraphEdiscoverySettings>: settings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: Read-only.
  - `[Ocr <IMicrosoftGraphEdiscoveryOcrSettings>]`: ocrSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabled <Boolean?>]`: 
    - `[MaxImageSize <Int32?>]`: 
    - `[Timeout <TimeSpan?>]`: 
  - `[RedundancyDetection <IMicrosoftGraphEdiscoveryRedundancyDetectionSettings>]`: redundancyDetectionSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabled <Boolean?>]`: 
    - `[MaxWords <Int32?>]`: 
    - `[MinWords <Int32?>]`: 
    - `[SimilarityThreshold <Int32?>]`: 
  - `[TopicModeling <IMicrosoftGraphEdiscoveryTopicModelingSettings>]`: topicModelingSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DynamicallyAdjustTopicCount <Boolean?>]`: 
    - `[IgnoreNumbers <Boolean?>]`: 
    - `[IsEnabled <Boolean?>]`: 
    - `[TopicCount <Int32?>]`: 

INPUTOBJECT <IComplianceIdentity>: Identity Parameter
  - `[CaseId <String>]`: key: id of case
  - `[CaseOperationId <String>]`: key: id of caseOperation
  - `[CustodianId <String>]`: key: id of custodian
  - `[DataSourceId <String>]`: key: id of dataSource
  - `[LegalHoldId <String>]`: key: id of legalHold
  - `[NoncustodialDataSourceId <String>]`: key: id of noncustodialDataSource
  - `[ReviewSetId <String>]`: key: id of reviewSet
  - `[ReviewSetQueryId <String>]`: key: id of reviewSetQuery
  - `[SiteSourceId <String>]`: key: id of siteSource
  - `[SourceCollectionId <String>]`: key: id of sourceCollection
  - `[TagId <String>]`: key: id of tag
  - `[UnifiedGroupSourceId <String>]`: key: id of unifiedGroupSource
  - `[UserSourceId <String>]`: key: id of userSource

OCR <IMicrosoftGraphEdiscoveryOcrSettings>: ocrSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsEnabled <Boolean?>]`: 
  - `[MaxImageSize <Int32?>]`: 
  - `[Timeout <TimeSpan?>]`: 

REDUNDANCYDETECTION <IMicrosoftGraphEdiscoveryRedundancyDetectionSettings>: redundancyDetectionSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsEnabled <Boolean?>]`: 
  - `[MaxWords <Int32?>]`: 
  - `[MinWords <Int32?>]`: 
  - `[SimilarityThreshold <Int32?>]`: 

TOPICMODELING <IMicrosoftGraphEdiscoveryTopicModelingSettings>: topicModelingSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DynamicallyAdjustTopicCount <Boolean?>]`: 
  - `[IgnoreNumbers <Boolean?>]`: 
  - `[IsEnabled <Boolean?>]`: 
  - `[TopicCount <Int32?>]`: 

## RELATED LINKS
