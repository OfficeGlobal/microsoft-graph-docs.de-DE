# <a name="educationstudent-resource-type"></a>educationStudent-Ressourcentyp

Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|birthDate|Datum| Geburtsdatum des Kursteilnehmers.|
|externalId|Zeichenfolge| ID des Kursteilnehmers im Quellsystem.|
|gender|educationGender| Die möglichen Werte sind: `female`, `male`, `other`, `unknownFutureValue`.|
|Ergebnis|Zeichenfolge|Aktuelle Klassenstufe des Kursteilnehmers.|
|graduationYear|Zeichenfolge| Jahr, in dem der Kursteilnehmer die Schule abschließt.|
|studentNumber|Zeichenfolge| Kursteilnehmernummer|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
