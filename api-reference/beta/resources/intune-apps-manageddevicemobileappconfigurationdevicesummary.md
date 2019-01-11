---
title: managedDeviceMobileAppConfigurationDeviceSummary-Ressourcentyp
description: Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Gerätestatus von MDM-Konfigurationen mobiler Apps.
localization_priority: Normal
ms.openlocfilehash: e395f0d3d1ceeacf9eb02c621eb0fbd7a30da907
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862622"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a>managedDeviceMobileAppConfigurationDeviceSummary-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Gerätestatus von MDM-Konfigurationen mobiler Apps.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurationDeviceSummary abrufen](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)-Objekts.|
|[managedDeviceMobileAppConfigurationDeviceSummary aktualisieren](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|pendingCount|Int32|Anzahl der ausstehenden Geräte|
|notApplicableCount|Int32|Anzahl der ausgenommenen Geräte|
|notApplicablePlatformCount|Int32|Anzahl der Geräte, die aufgrund von Konflikt Plattform und Richtlinie nicht zutreffend|
|successCount|Int32|Anzahl der erfolgreichen Geräte|
|errorCount|Int32|Anzahl der fehlerhaften Geräte|
|failedCount|Int32|Anzahl der fehlgeschlagenen Geräte|
|conflictCount|Int32|Anzahl der Geräte in Konflikt|
|lastUpdateDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Aktualisierung|
|configurationVersion|Int32|Version der Richtlinie für diese Übersicht|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





