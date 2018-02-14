# <a name="exclusiongroupassignmenttarget-resource-type"></a>exclusionGroupAssignmentTarget-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.

Erbt von [groupAssignmentTarget](../resources/intune_deviceconfig_groupassignmenttarget.md).

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|groupId|Zeichenfolge|Die Gruppen-ID, die das Ziel der Zuweisung ist. Vererbt von [groupAssignmentTarget](../resources/intune_deviceconfig_groupassignmenttarget.md).|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



