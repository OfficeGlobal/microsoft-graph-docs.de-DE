# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>androidForWorkAppConfigurationSchemaItem-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Einzelnes Konfigurationselement in einem benutzerdefinierten Konfigurationsschema einer Android for Work-Anwendung.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|schemaItemKey|String|Eindeutiger Schlüssel, mit dem die Anwendung das Element identifiziert.|
|displayName|String|Lesbarer Name|
|description|String|Beschreibung dessen, was das Element innerhalb der Anwendung steuert.|
|defaultBoolValue|Boolean|Standardwert für boolesche Elemente, wenn vom App-Entwickler angegeben.|
|defaultIntValue|Int32|Standardwert für Elemente vom Typ Integer, wenn vom App-Entwickler angegeben.|
|defaultStringValue|String|Standardwert für Elemente vom Typ String, wenn vom App-Entwickler angegeben.|
|defaultStringArrayValue|String-Sammlung|Standardwert für Elemente vom Typ String-Array, wenn vom App-Entwickler angegeben.|
|dataType|String|Der Typ des Werts, den dieses Element beschreibt. Mögliche Werte: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md)-Sammlung|Liste lesbarer Name-Wert-Paare für die gültigen Werte, die für dieses Element festgelegt werden können (nur Choice- und Multiselect-Elemente)|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



