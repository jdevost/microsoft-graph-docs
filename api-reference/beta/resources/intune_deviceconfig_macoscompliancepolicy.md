﻿# macOSCompliancePolicy resource type> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.

This class contains compliance settings for Mac OS.

Inherits from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

### Methods
|Method|Return Type|Description|
|---|---|---|
|[List macOSCompliancePolicies](../api/intune_deviceconfig_macoscompliancepolicy_list.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) collection|List properties and relationships of the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) objects.|
|[Get macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_get.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Read properties and relationships of the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.|
|[Create macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_create.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Create a new [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.|
|[Delete macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_delete.md)|None|Deletes a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Update macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_update.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Update the properties of a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.|
|[List deviceCompliancePolicyGroupAssignments](../api/intune_deviceconfig_macoscompliancepolicy_list_devicecompliancepolicygroupassignment.md)|[deviceCompliancePolicyGroupAssignment](../resources/intune_deviceconfig_devicecompliancepolicygroupassignment.md) collection|Get the deviceCompliancePolicyGroupAssignments from the groupAssignments navigation property.|
|[List deviceComplianceScheduledActionForRules](../api/intune_deviceconfig_macoscompliancepolicy_list_devicecompliancescheduledactionforrule.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[List deviceComplianceDeviceStatuses](../api/intune_deviceconfig_macoscompliancepolicy_list_devicecompliancedevicestatus.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) collection|Get the deviceComplianceDeviceStatuses from the deviceStatuses navigation property.|
|[List deviceComplianceUserStatuses](../api/intune_deviceconfig_macoscompliancepolicy_list_devicecomplianceuserstatus.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|

### Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordRequired|Boolean|Whether or not to require a password.|
|passwordBlockSimple|Boolean|Indicates whether or not to block simple passwords.|
|passwordExpirationDays|Int32|Number of days before the password expires.|
|passwordMinimumLength|Int32|Minimum length of passwords.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutes of inactivity required before a password is required.|
|passwordPreviousPasswordBlockCount|Int32|Number of previous passwords to block.|
|passwordRequiredType|String|Type of password that is required. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|

### Relationships
|Relationship|Type|Description|
|---|---|---|
|groupAssignments|[deviceCompliancePolicyGroupAssignment](../resources/intune_deviceconfig_devicecompliancepolicygroupassignment.md) collection|The list of group assignments for this compliance policy. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) collection|The list of scheduled action for this rule Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) collection|List of DeviceComplianceDeviceStatus. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) collection|List of DeviceComplianceUserStatus. Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

### JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSCompliancePolicy"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String"
}
```



