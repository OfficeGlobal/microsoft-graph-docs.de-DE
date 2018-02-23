# <a name="androidforworkappconfigurationschema-resource-type"></a>androidForWorkAppConfigurationSchema-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Schema, das die benutzerdefinierten Konfigurationen für eine Android for Work-Anwendung beschreibt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[androidForWorkAppConfigurationSchemas auflisten](../api/intune_androidforwork_androidforworkappconfigurationschema_list.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Sammlung|Listet die Eigenschaften und Beziehungen [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Objekten auf.|
|[androidForWorkAppConfigurationSchema abrufen](../api/intune_androidforwork_androidforworkappconfigurationschema_get.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Listet die Eigenschaften und Beziehungen des [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Objekts auf.|
|[androidForWorkAppConfigurationSchema erstellen](../api/intune_androidforwork_androidforworkappconfigurationschema_create.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Erstellen eines neuen [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Objekts.|
|[androidForWorkAppConfigurationSchema löschen](../api/intune_androidforwork_androidforworkappconfigurationschema_delete.md)|Keine|Löschen eines [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).|
|[androidForWorkAppConfigurationSchema aktualisieren](../api/intune_androidforwork_androidforworkappconfigurationschema_update.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Aktualisieren der Eigenschaften eines [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel für die Entität des Android-Paketnamens der Anwendung, die dem Schema entspricht|
|exampleJson|Binär|UTF8-codiertes Bytearray mit diesem Schema entsprechender Beispiel-JSON-Zeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden muss|
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md)-Sammlung|Sammlung von Elementen, von denen jedes eine benannte Konfigurationsoption im Schema darstellt.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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
  ]
}
```



