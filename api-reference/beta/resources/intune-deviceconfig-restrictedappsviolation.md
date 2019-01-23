---
title: Ressourcentyp restrictedAppsViolation
description: Verletzung der eingeschränkten apps Konfigurationsprofil pro Gerät pro Benutzer
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcbd7def59d17dcd6e906e1e6bef85e3a448b880
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424980"
---
# <a name="restrictedappsviolation-resource-type"></a>Ressourcentyp restrictedAppsViolation

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




