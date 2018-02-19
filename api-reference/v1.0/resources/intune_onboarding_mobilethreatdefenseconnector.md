# <a name="mobilethreatdefenseconnector-resource-type"></a>Ressourcentyp „mobileThreatDefenseConnector“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die eine Verbindung zu einem Mobile Threat Defense-Partner repräsentiert
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mobileThreatDefenseConnector“](../api/intune_onboarding_mobilethreatdefenseconnector_list.md)|Sammlung von Ressourcen des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) auf.|
|[Abrufen von „mobileThreatDefenseConnector“](../api/intune_onboarding_mobilethreatdefenseconnector_get.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Erstellen von „mobileThreatDefenseConnector“](../api/intune_onboarding_mobilethreatdefenseconnector_create.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Löschen von „mobileThreatDefenseConnector“](../api/intune_onboarding_mobilethreatdefenseconnector_delete.md)|Keiner|Löscht Objekte des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Aktualisieren von „mobileThreatDefenseConnector“](../api/intune_onboarding_mobilethreatdefenseconnector_update.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Aktualisiert die Eigenschaften von Objekten des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|lastHeartbeatDateTime|DateTimeOffset|Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to MTP“ durch den Administrator|
|partnerState|String|Partnerstatus des Mandanten. Mögliche Werte sind: `unavailable`, `available`, `enabled` und `unresponsive`.|
|androidEnabled|Boolean|Aktiviert oder deaktiviert Android.|
|androidDeviceBlockedOnMissingPartnerData|Boolean|Für Android. Erlaubt es dem Administrator, festzulegen, dass Daten vom Datensynchronisierungspartner empfangen werden müssen, bevor Konformität angenommen wird.|
|iosDeviceBlockedOnMissingPartnerData|Boolean|Für iOS. Erlaubt es dem Administrator, festzulegen, dass Daten vom Datensynchronisierungspartner empfangen werden müssen, bevor Konformität angenommen wird.|
|partnerUnsupportedOsVersionBlocked|Boolean|Erlaubt es dem Administrator, Geräte mit den aktivierten Plattformen zu blockieren, wenn sie die Mindestanforderungen an die Version nicht erfüllen.|
|iosEnabled|Boolean|Aktiviert oder deaktiviert iOS.|
|partnerUnresponsivenessThresholdInDays|Int32|Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
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
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```



