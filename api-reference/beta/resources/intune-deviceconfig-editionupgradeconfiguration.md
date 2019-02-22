---
title: editionUpgradeConfiguration-Ressourcentyp
description: Editionsupgradekonfiguration Windows 10
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ef28f1893e3a4654e92db6e1569f546e38c9746
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162951"
---
# <a name="editionupgradeconfiguration-resource-type"></a>editionUpgradeConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Editionsupgradekonfiguration Windows 10


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[editionUpgradeConfigurations auflisten](../api/intune-deviceconfig-editionupgradeconfiguration-list.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)-Objekte.|
|[editionUpgradeConfiguration abrufen](../api/intune-deviceconfig-editionupgradeconfiguration-get.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)-Objekts.|
|[editionUpgradeConfiguration erstellen](../api/intune-deviceconfig-editionupgradeconfiguration-create.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Erstellen eines neuen [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)-Objekts.|
|[editionUpgradeConfiguration löschen](../api/intune-deviceconfig-editionupgradeconfiguration-delete.md)|Keine|Löscht eine [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).|
|[editionUpgradeConfiguration aktualisieren](../api/intune-deviceconfig-editionupgradeconfiguration-update.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|Aktualisieren der Eigenschaften eines [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|licenseType|[editionUpgradeLicenseType](../resources/intune-deviceconfig-editionupgradelicensetype.md)|Typ der Edition Upgrade-Lizenz. Mögliche Werte sind: `productKey`, `licenseFile` und `notConfigured`.|
|targetEdition|[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)|Zieledition von Edition Upgrade. Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education` `windows10EducationN`,, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional` `windows10ProfessionalN`,, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN`,, `notConfigured`.|
|license|Zeichenfolge|Inhalt der Edition Upgrade-Lizenzdatei|
|productKey|Zeichenfolge|Product Key von Edition Upgrade|
|windowsSMode|[windowsSModeConfiguration](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|Konfiguration des S-Modus. Mögliche Werte sind: `noRestriction`, `block` und `unlock`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.editionUpgradeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "String",
  "productKey": "String",
  "windowsSMode": "String"
}
```




