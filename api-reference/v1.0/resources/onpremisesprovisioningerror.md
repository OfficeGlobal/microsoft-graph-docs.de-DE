# <a name="onpremisesprovisioningerror-resource-type"></a>Ressourcentyp onPremisesProvisioningError

Repräsentiert Verzeichnissynchronisierungsfehler bei der Synchronisierung lokaler Verzeichnisse zum Azure Active Directory für die [Benutzer-](user.md) und [Gruppe](group.md)-Entitäten.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|Kategorie|Zeichenfolge| Die Kategorie des Provisioning-Fehler. Hinweis: Zurzeit besteht nur ein möglicher Wert. Möglicher Wert: *PropertyConflict* - gibt an, dass ein Eigenschaftswert nicht eindeutig ist. Andere Objekte enthalten den gleichen Wert für die Eigenschaft. |
|occurredDateTime|DateTimeOffset| Das Datum und die Uhrzeit, an denen der Fehler aufgetreten ist. |
|propertyCausingError|Zeichenfolge| Name der Verzeichniseigenschaft, die den Fehler verursacht. Aktuelle mögliche Werte: *UserPrincipalName* oder *ProxyAddress* |
|Wert|Zeichenfolge| Der Wert der Eigenschaft, die den Fehler verursacht. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->