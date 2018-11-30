---
title: Ressourcentyp restrictedAppsViolation
description: Verletzung der eingeschränkten apps Konfigurationsprofil pro Gerät pro Benutzer
ms.openlocfilehash: 6d7f6cb8b52671c311c39c3306a329ad37194b85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064347"
---
# <a name="restrictedappsviolation-resource-type"></a>Ressourcentyp restrictedAppsViolation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verletzung der eingeschränkten apps Konfigurationsprofil pro Gerät pro Benutzer
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Auflistung|Listeneigenschaften und Beziehungen der [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekte.|
|[Abrufen von restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Lesen Sie Eigenschaften und Beziehungen des [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|
|[Erstellen von restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Erstellen eines neuen [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|
|[RestrictedAppsViolation löschen](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Keines|Löscht eine [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[RestrictedAppsViolation aktualisieren](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Aktualisieren Sie die Eigenschaften eines [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Objekt. Besteht aus den AccountId, Geräte-ID, PolicyId und Benutzer-ID|
|userId|String|Eindeutige Benutzer-ID muss Guid|
|userName|String|Benutzername|
|managedDeviceId|String|Eindeutiger Bezeichner der verwalteten Gerät, muss die Guid|
|deviceName|String|Gerätename|
|deviceConfigurationId|String|Gerät Konfiguration Profil Eindeutiger Bezeichner muss Guid|
|deviceConfigurationName|String|Gerätename Konfiguration-Profil|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Plattformtyp. Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Eingeschränkte apps Zustand. Mögliche Werte sind: `prohibitedApps` und `notApprovedApps`.|
|restrictedApps|[ManagedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) -Auflistung|Liste der verletzte eingeschränkte apps|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```





