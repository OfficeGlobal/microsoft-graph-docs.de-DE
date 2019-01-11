---
title: Ressourcentyp restrictedAppsViolation
description: Verletzung der eingeschränkten apps Konfigurationsprofil pro Gerät pro Benutzer
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aefd9996805f0ee454bebc8871662b0ceac05a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849378"
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
|[RestrictedAppsViolation löschen](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Keine|Löscht eine [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[RestrictedAppsViolation aktualisieren](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Aktualisieren Sie die Eigenschaften eines [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Objekt. Besteht aus den AccountId, Geräte-ID, PolicyId und Benutzer-ID|
|userId|Zeichenfolge|Eindeutige Benutzer-ID muss Guid|
|userName|Zeichenfolge|Benutzername|
|managedDeviceId|Zeichenfolge|Eindeutiger Bezeichner der verwalteten Gerät, muss die Guid|
|deviceName|Zeichenfolge|Gerätename|
|deviceConfigurationId|Zeichenfolge|Gerät Konfiguration Profil Eindeutiger Bezeichner muss Guid|
|deviceConfigurationName|Zeichenfolge|Gerätename Konfiguration-Profil|
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





