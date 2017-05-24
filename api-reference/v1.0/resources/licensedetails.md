# <a name="licensedetails-resource-type"></a>licenseDetails-Ressourcentyp

Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.

### <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[licenseDetails auflisten](../api/user_list_licensedetails.md) | licenseDetails-Sammlung |Dient zum Abrufen einer Liste von licenseDetails-Objekten für einen Benutzer.|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Der eindeutige Bezeichner für das licenseDetails-Objekt. Schreibgeschützt, Schlüssel, lässt keine Nullwerte zu. |
|servicePlans|[servicePlanInfo](serviceplaninfo.md)-Sammlung| Informationen über die Servicepläne, die mit der Lizenz zugewiesen werden. Schreibgeschützt, lässt keine Nullwerte zu. |
|skuId|Guid| Der eindeutige Bezeichner (GUID) für die Dienst-SKU. Entspricht der skuId-Eigenschaft des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts. Schreibgeschützt |
|skuPartNumber|String| Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt |

### <a name="relationships"></a>Beziehungen
Keine

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->