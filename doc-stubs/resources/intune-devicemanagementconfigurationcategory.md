---
title: "deviceManagementConfigurationCategory resource type"
description: "Device Management Configuration Policy"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementConfigurationCategory resource type

Namespace: microsoft.graph

Device Management Configuration Policy

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceManagementConfigurationCategories](../api/intune-devicemanagementconfigurationcategory-list.md)|[deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md) collection|Get a list of the [deviceManagementConfigurationCategory](../resources/devicemanagementconfigurationcategory.md) objects and their properties.|
|[Create deviceManagementConfigurationCategory](../api/intune-devicemanagementconfigurationcategory-create.md)|[deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md)|Create a new [deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md) object.|
|[Get deviceManagementConfigurationCategory](../api/intune-devicemanagementconfigurationcategory-get.md)|[deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md)|Read the properties and relationships of a [deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md) object.|
|[Update deviceManagementConfigurationCategory](../api/intune-devicemanagementconfigurationcategory-update.md)|[deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md)|Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md) object.|
|[Delete deviceManagementConfigurationCategory](../api/intune-devicemanagementconfigurationcategory-delete.md)|None|Deletes a [deviceManagementConfigurationCategory](../resources/intune-devicemanagementconfigurationcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childCategoryIds|String collection|List of child ids of the category.|
|description|String|Description of the item|
|displayName|String|Display name of the item|
|helpText|String|Help text of the item|
|id|String|Identifier for item|
|name|String|Name of the item|
|parentCategoryId|String|Parent id of the category.|
|platforms|deviceManagementConfigurationPlatforms|Platforms types, which settings in the category have. Possible values are: `none`, `macOS`, `windows10X`, `windows10`.|
|rootCategoryId|String|Root id of the category.|
|settingUsage|deviceManagementConfigurationSettingUsage|Indicates that the category contains settings that are used for Compliance or Configuration. Possible values are: `none`, `configuration`.|
|technologies|deviceManagementConfigurationTechnologies|Technologies types, which settings in the category have. Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationCategory",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "platforms": "String",
  "technologies": "String",
  "settingUsage": "String",
  "parentCategoryId": "String",
  "rootCategoryId": "String",
  "childCategoryIds": [
    "String"
  ]
}
```
