# <a name="applepushnotificationcertificate-resource-type"></a>applePushNotificationCertificate-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Apple Push Notification-Zertifikat.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[applePushNotificationCertificate abrufen](../api/intune_devices_applepushnotificationcertificate_get.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Lesen von Eigenschaften und Beziehungen des [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)-Objekts.|
|[applePushNotificationCertificate aktualisieren](../api/intune_devices_applepushnotificationcertificate_update.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Aktualisieren der Eigenschaften eines [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)-Objekts.|
|[downloadApplePushNotificationCertificateSigningRequest-Funktion](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|String|Signieranforderung für Apple Push Notification-Zertifikat herunterladen|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Zertifikat|
|appleIdentifier|String|Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde.|
|topicIdentifier|String|Thema-ID|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -Uhrzeit für das Apple Push Notification-Zertifikat.|
|certificate|String|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



