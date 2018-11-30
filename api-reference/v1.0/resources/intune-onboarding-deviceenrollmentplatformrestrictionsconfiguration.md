---
title: deviceEnrollmentPlatformRestrictionsConfiguration-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: d49c4a94b36593204abd92567b2ea1855527deb6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018625"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a>deviceEnrollmentPlatformRestrictionsConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.

Erbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceEnrollmentPlatformRestrictionsConfigurations auflisten](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekte.|
|[DeviceEnrollmentPlatformRestrictionsConfiguration abrufen](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.|
|[DeviceEnrollmentPlatformRestrictionsConfiguration erstellen](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.|
|[DeviceEnrollmentPlatformRestrictionsConfiguration löschen](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|Keine|Löscht ein [DeviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekt.|
|[DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|Priorität|Int32|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|Version|Int32|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|iosRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Noch nicht dokumentiert.|
|windowsRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Noch nicht dokumentiert.|
|windowsMobileRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Noch nicht dokumentiert.|
|androidRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Noch nicht dokumentiert.|
|macOSRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  }
}
```



