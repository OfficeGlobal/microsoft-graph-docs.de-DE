# <a name="multivaluelegacyextendedproperty-resource-type"></a>multiValueLegacyExtendedProperty-Ressourcentyp

Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.

Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Beitrag](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md). Beachten Sie, dass [post](../resources/post.md) für die Gruppe nicht unterstützt wird. | Erstellen einer **multiValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource. |
|[Get](../api/multivaluelegacyextendedproperty_get.md) |Eine unterstützte Ressourceninstanz ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe), erweitert mit einem [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Objekt. |Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand`.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge|Die Eigenschaften-ID. Schreibgeschützt.|
|value|string collection|Eine Sammlung von Eigenschaftswerten.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->