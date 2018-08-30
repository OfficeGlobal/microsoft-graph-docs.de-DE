# <a name="inferenceclassification-resource-type"></a>inferenceClassification-Ressourcentyp

Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind. 

Weitere Informationen finden Sie unter [Posteingang mit Relevanz verwalten](manage_focused_inbox.md).


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[inferenceClassificationOverride erstellen](../api/inferenceclassification_post_overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md)| Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.|
|[Außerkraftsetzungen auflisten](../api/inferenceclassification_list_overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md)-Sammlung| Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ID|Zeichenfolge| Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Außerkraftsetzungen|[inferenceClassificationOverride](inferenceclassificationoverride.md)-Sammlung| Eine Reihe von Außerkraftsetzungen für einen Benutzer, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren: `focused` oder `other`. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->