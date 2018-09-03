# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride-Ressourcentyp

Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Aktualisieren](../api/inferenceclassificationoverride_update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben. |
|[Löschen](../api/inferenceclassificationoverride_delete.md) | Keine |Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| Gibt an, wie eingehende Nachrichten von einem bestimmten Absender stets klassifiziert werden sollen. Die möglichen Werte sind: `focused`, `other`.|
|id|Zeichenfolge| Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.|
|senderEmailAddress|[emailAddress](emailaddress.md)|Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->