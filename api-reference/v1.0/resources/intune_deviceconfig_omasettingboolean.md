# <a name="omasettingboolean-resource-type"></a>omaSettingBoolean-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Boolesche Definition der OMA-Einstellungen.

Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|Zeichenfolge|Beschreibung. Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|Zeichenfolge|OMA Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|Wert|Boolescher|Wert.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```








