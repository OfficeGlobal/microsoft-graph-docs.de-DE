# <a name="cloudappsecuritystate-resource-type"></a>Ressourcentyp cloudAppSecurityState

Enthält Zustandsinformationen über die Cloud-Anwendung (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|destinationServiceIp|Zeichenfolge|Ziel-IP-Adresse der Verbindung mit der Cloud-Anwendung/dem Dienst.|
|destinationServiceName|Zeichenfolge|Name der Cloud-Anwendung/des Dienstes (zum Beispiel "Salesforce", "DropBox" usw.).|
|riskScore|Zeichenfolge|Vom Anbieter generierte/berechnete Risikobewertung der Cloud-Anwendung/des Dienstes. Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->