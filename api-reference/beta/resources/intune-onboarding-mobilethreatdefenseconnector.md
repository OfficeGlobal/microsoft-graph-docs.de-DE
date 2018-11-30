---
title: Ressourcentyp „mobileThreatDefenseConnector“
description: Entität, die eine Verbindung zu einem Mobile Threat Defense-Partner repräsentiert
ms.openlocfilehash: ee832f8e3acce151d51483522aa0c76b181e93d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061773"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>Ressourcentyp „mobileThreatDefenseConnector“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die eine Verbindung zu einem Mobile Threat Defense-Partner repräsentiert
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mobileThreatDefenseConnector“](../api/intune-onboarding-mobilethreatdefenseconnector-list.md)|Sammlung von Ressourcen des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) auf.|
|[Abrufen von „mobileThreatDefenseConnector“](../api/intune-onboarding-mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Erstellen von „mobileThreatDefenseConnector“](../api/intune-onboarding-mobilethreatdefenseconnector-create.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Löschen von „mobileThreatDefenseConnector“](../api/intune-onboarding-mobilethreatdefenseconnector-delete.md)|Keiner|Löscht Objekte des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Aktualisieren von „mobileThreatDefenseConnector“](../api/intune-onboarding-mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Aktualisiert die Eigenschaften von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|lastHeartbeatDateTime|DateTimeOffset|DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Daten Sync Partner Zustand für dieses Konto. Mögliche Werte: sind `unavailable`, `available`, `enabled` und `unresponsive`.|
|androidEnabled|Boolean|Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.|
|iosEnabled|Boolean|Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.|
|windowsEnabled|Boolesch|Abzurufen Sie für Windows oder festzulegen Sie, ob die Daten aus der Daten Sync Partner beim Testen der Kompatibilität verwendet werden soll|
|macEnabled|Boolesch|Abzurufen Sie für Mac oder festzulegen Sie, ob die Daten aus der Daten Sync Partner beim Testen der Kompatibilität verwendet werden soll|
|androidDeviceBlockedOnMissingPartnerData|Boolean|Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.|
|iosDeviceBlockedOnMissingPartnerData|Boolean|Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.|
|windowsDeviceBlockedOnMissingPartnerData|Boolesch|Festlegen Sie für Windows, ob Intune Daten vom Partner Sync Daten vor der Markierung ein Gerät kompatible empfangen muss|
|macDeviceBlockedOnMissingPartnerData|Boolesch|Abzurufen Sie für Mac oder festzulegen Sie, ob Intune Daten vom Partner Sync Daten vor der Markierung ein Gerät kompatible empfangen muss|
|partnerUnsupportedOsVersionBlocked|Boolean|Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.|
|partnerUnresponsivenessThresholdInDays|Int32|Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.|
|allowPartnerToCollectIOSApplicationMetadata|Boolesch|IOS-Geräte ermöglicht den Administrator konfigurieren können, ob der Daten Sync Partner auch Metadaten für die installierten Programme auf Intune erfassen möglicherweise|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```





