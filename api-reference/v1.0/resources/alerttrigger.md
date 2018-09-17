# <a name="alerttrigger-resource-type"></a>Ressourcentyp alertTrigger

Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst haben (Eigenschaften sind in der Warnungsentität vorhanden).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|Name|Zeichenfolge|Der Name der Eigenschaft, der als ein Erkennungstrigger gedient hat.|
|Typ|Zeichenfolge|Typ der Eigenschaft im Schlüssel/Wert-Paar für die Auslegung. Bspw. String, Boolean, usw.|
|Wert|Zeichenfolge|Der Wert der Eigenschaft, der als ein Erkennungstrigger gedient hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>Beispiel

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->