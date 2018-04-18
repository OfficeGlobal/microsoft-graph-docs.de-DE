# <a name="privacyprofile-resource-type"></a>privacyProfile-Ressourcentyp

Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|contactEmail|Zeichenfolge| Eine gültige SMTP-E-Mail-Adresse für den Kontakt für die Datenschutzerklärung Nicht erforderlich.|
|statementUrl|Zeichenfolge| Ein gültiges URL-Format, das mit „http://“ oder „https://“ beginnt. Die maximale Länge beträgt 255 Zeichen. Die URL, die zur Datenschutzerklärung des Unternehmens weiterleitet. Nicht erforderlich.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```