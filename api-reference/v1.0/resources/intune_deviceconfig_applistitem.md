# <a name="applistitem-resource-type"></a>appListItem-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt eine App in der Liste der verwalteten Anwendungen dar.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Anwendungsname|
|publisher|Zeichenfolge|Herausgeber der App|
|appStoreUrl|Zeichenfolge|Store-URL der Anwendung|
|appId|Zeichenfolge|Anwendungs- oder Paket-ID der Anwendung|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



