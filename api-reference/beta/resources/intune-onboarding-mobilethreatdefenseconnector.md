---
title: Ressourcentyp „mobileThreatDefenseConnector“
description: Entität, die eine Verbindung zu einem Mobile Threat Defense-Partner repräsentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b76d7f0db09d1fd945a2d4588c4268e07b19b14
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161733"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>Ressourcentyp „mobileThreatDefenseConnector“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|Zeichenfolge|Noch nicht dokumentiert|
|lastHeartbeatDateTime|DateTimeOffset|DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Daten Synchronisierungs Partner Status für dieses Konto. Mögliche Werte: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidEnabled|Boolescher Wert|Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.|
|iosEnabled|Boolescher Wert|Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.|
|windowsEnabled|Boolescher Wert|Für Windows: Abrufen oder festlegen, ob Daten vom Daten Synchronisierungspartner während der Konformitätsbewertung verwendet werden sollen|
|macEnabled|Boolescher Wert|Für Mac: Abrufen oder festlegen, ob Daten vom Daten Synchronisierungspartner während der Konformitätsbewertung verwendet werden sollen|
|androidDeviceBlockedOnMissingPartnerData|Boolescher Wert|Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.|
|iosDeviceBlockedOnMissingPartnerData|Boolean|Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.|
|windowsDeviceBlockedOnMissingPartnerData|Boolescher Wert|Legen Sie unter Windows fest, ob InTune Daten vom Daten Synchronisierungspartner empfangen muss, bevor ein Gerät kompatibel markiert wird.|
|macDeviceBlockedOnMissingPartnerData|Boolescher Wert|Für Mac: Abrufen oder festlegen, ob InTune Daten vom Daten Synchronisierungspartner empfangen muss, bevor ein Gerät kompatibel markiert wird.|
|partnerUnsupportedOsVersionBlocked|Boolean|Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.|
|partnerUnresponsivenessThresholdInDays|Int32|Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.|
|allowPartnerToCollectIOSApplicationMetadata|Boolescher Wert|Ermöglicht dem Administrator für IOS-Geräte, zu konfigurieren, ob der Daten Synchronisierungspartner auch Metadaten zu installierten Anwendungen von InTune erfassen kann.|

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




