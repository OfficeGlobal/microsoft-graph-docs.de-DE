# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Konfiguration der geplanten Aktivität
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceActionItems auflisten](../api/intune_deviceconfig_devicecomplianceactionitem_list.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Objekte.|
|[deviceComplianceActionItem abrufen](../api/intune_deviceconfig_devicecomplianceactionitem_get.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Objekts.|
|[deviceComplianceActionItem erstellen](../api/intune_deviceconfig_devicecomplianceactionitem_create.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Erstellen eines neuen [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Objekts.|
|[deviceComplianceActionItem löschen](../api/intune_deviceconfig_devicecomplianceactionitem_delete.md)|Keine|Löschen eines [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[deviceComplianceActionItem aktualisieren](../api/intune_deviceconfig_devicecomplianceactionitem_update.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|gracePeriodHours|Int32|Die Anzahl der Stunden, bis die Aktion erzwungen wird. Gültige Werte: 0 bis 8760|
|actionType|Zeichenfolge|Mögliche Werte für den Aktionstyp: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.|
|notificationTemplateId|Zeichenfolge|Auswahl der verwendeten Benachrichtigungsvorlage|
|notificationMessageCCList|Zeichenfolgenauflistung|Eine Liste der Gruppen-IDs, die festlegt, wer bei dieser Benachrichtigung auf „CC“ gesetzt wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



