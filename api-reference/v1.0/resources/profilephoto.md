# <a name="profilephoto-resource-type"></a>profilePhoto-Ressourcentyp
Ein Profilfoto eines Benutzers, einer Gruppe oder eines Outlook-Kontakts, auf den bzw. die von Exchange Online zugegriffen wird. Es handelt sich um Binärdaten, die nicht in Base-64 codiert sind.

Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“. 

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[profilePhoto abrufen](../api/profilephoto_get.md) | [profilePhoto](profilephoto.md) |Ruft das angegebene **profilePhoto** oder seine Metadaten (profilePhoto-Eigenschaften) ab.|
|[Update](../api/profilephoto_update.md) | [profilePhoto](profilephoto.md)  |Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden).|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Schreibgeschützt.|
|height|int32|Die Höhe des Fotos. Schreibgeschützt.|
|width|int32|Die Breite des Fotos. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
