# <a name="devicecompliancescheduledactionforrule-resource-type"></a>deviceComplianceScheduledActionForRule-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Geplante Aktion für eine Regel
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceScheduledActionForRules auflisten](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_list.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) collection|Auflisten von Eigenschaften und Beziehungen der [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)-Objekte.|
|[deviceComplianceScheduledActionForRule abrufen](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_get.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)-Objekts.|
|[deviceComplianceScheduledActionForRule erstellen](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_create.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Erstellen eines neuen [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)-Objekts.|
|[deviceComplianceScheduledActionForRule löschen](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_delete.md)|Keine|Löscht ein [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)-Objekt.|
|[deviceComplianceScheduledActionForRule aktualisieren](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_update.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Aktualisieren der Eigenschaften eines [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|ruleName|String|Name der Regel, für die diese geplante Aktion gilt.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Sammlung|Die Liste der geplanten Aktionskonfigurationen für diese Compliance-Richtlinie.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```



