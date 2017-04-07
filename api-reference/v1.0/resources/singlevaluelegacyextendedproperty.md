# <a name="singlevaluelegacyextendedproperty-resource-type"></a>singleValueLegacyExtendedProperty-Ressourcentyp

Eine erweiterte Eigenschaft, die einen einzelnen Wert enthält. 

Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden. 


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md), aber nicht [post](../resources/post.md) für die Gruppe. | Erstellen einer **singleValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource. |
|[Get](../api/singlevaluelegacyextendedproperty_get.md) |Eine unterstützte Ressourceninstanz oder eine Sammlung von unterstützten Ressourceninstanzen ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe) oder eine solche Instanz erweitert mit einem [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Objekt. |Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` oder `$filter`.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Die Eigenschafts-ID, die zum Identifizieren der Eigenschaft verwendet wird. Schreibgeschützt.|
|value|string|Ein Eigenschaftswert.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singlevaluelegacyextendedproperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->