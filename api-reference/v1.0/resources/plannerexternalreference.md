# <a name="plannerexternalreference-resource-type"></a>plannerExternalReference-Ressourcentyp

Die **plannerExternalReference**-Ressource stellt die Metadaten eines Verweises dar (Anlagen wie z. B. Datei, URL). Es ist der Wert von Eigenschaft-Wert-Paaren im [externalReferences](plannerexternalreferences.md)-Objekt.



### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|alias|String|Ein Namensalias zur Beschreibung des Verweises.|
|lastModifiedBy|[identitySet](identityset.md)|Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.|
|lastModifiedDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|previewPriority|String|Wird verwendet, um die relative Prioritätsreihenfolge festzulegen, in der der Verweis als Vorschau für die Aufgaben angezeigt wirdd.|
|type|String|Wird verwendet, um den Verweis zu beschreiben. Zu den Typen gehören: `PowerPoint`, `Word`, `Excel`, `Other`.|

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->