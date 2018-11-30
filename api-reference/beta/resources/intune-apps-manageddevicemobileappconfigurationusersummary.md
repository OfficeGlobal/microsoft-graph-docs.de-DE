---
title: managedDeviceMobileAppConfigurationUserSummary-Ressourcentyp
description: Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Benutzerstatus von MDM-Konfigurationen mobiler Apps.
ms.openlocfilehash: b27f4c24dc4b89238ec4e555d9507f36795ebc9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061045"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a>managedDeviceMobileAppConfigurationUserSummary-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Benutzerstatus von MDM-Konfigurationen mobiler Apps.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurationUserSummary abrufen](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)-Objekts.|
|[managedDeviceMobileAppConfigurationUserSummary aktualisieren](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|pendingCount|Int32|Anzahl der ausstehenden Benutzer|
|notApplicableCount|Int32|Anzahl der Benutzer nicht zutreffend|
|successCount|Int32|Anzahl der erfolgreichen Benutzer|
|errorCount|Int32|Anzahl der Benutzer mit Fehlern|
|failedCount|Int32|Anzahl der fehlgeschlagenen Benutzer|
|conflictCount|Int32|Anzahl von Benutzern in Konflikt|
|lastUpdateDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Aktualisierung|
|configurationVersion|Int32|Version der Richtlinie für diese Übersicht|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





