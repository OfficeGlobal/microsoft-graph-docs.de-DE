# <a name="contract-resource-type"></a>Contract-Ressourcentyp
Stellt eine bestehende Partnerschaft zwischen dem Partnermandanten und einem Kundenmandanten dar.

> **Wichtig:** Ist nur in Partnermandanten vorhanden. Partnermandanten sind Azure AD-Mandanten, die zu Microsoft-Partnern gehören, die Teil der Partnerprogramme [Microsoft Cloud-Lösungsanbieter](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication oder Microsoft Advisor sind.

### <a name="methods"></a>Methoden

| Methode   | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Vertrag abrufen](../api/contract_get.md) | Contract |Dient zum Lesen der Eigenschaften eines bestimmten Vertragsobjekts. |
|[Verträge auflisten](../api/contract_list.md) | Contract-Sammlung | Liste der Verträge im Partnermandanten. |

### <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
|contractType|String|Typ des Vertrags.<br><br>Die folgenden Werte sind möglich:<br> *SyndicationPartner*: Partner, der Office 365 und Intune exklusiv für diesen Kunden verkauft und verwaltet. Die Partner verkaufen und erbringen Supportleistungen für ihre Kunden.<br> *BreadthPartner*: Partner, der administrative Unterstützung für diesen Kunden bereitstellen kann. Der Partner darf jedoch nicht an den Kunden verkaufen.<br>*ResellerPartner*: Ähnlicher Partner wie Syndication-Partner, mit der Ausnahme, dass der Partner keinen exklusiven Zugriff auf einen Mandanten hat. Im Syndication-Fall kann der Kunde keine zusätzlichen direkten Abonnements von Microsoft oder von anderen Partnern kaufen.|
|customerId|Guid|Der eindeutige Bezeichner für den Kundenmandanten, auf den in dieser Partnerschaft verwiesen wird. Entspricht der id-Eigenschaft der organization-Ressource des Kundenmandanten. |
|defaultDomainName|String|Eine Kopie des Standarddomänennamens des Kundenmandanten. Die Kopie wird erstellt, wenn die Partnerschaft mit dem Kunden eingerichtet wird. Sie wird nicht automatisch aktualisiert, wenn sich der Standarddomänenname des Kundenmandanten ändert.|
|displayName|String|Eine Kopie des Anzeigenamens des Kundenmandanten. Die Kopie wird erstellt, wenn die Partnerschaft mit dem Kunden eingerichtet wird. Sie wird nicht automatisch aktualisiert, wenn sich der Anzeigenname des Kundenmandanten ändert.|
|id|String| Der eindeutige Bezeichner für die Partnerschaft. Schlüssel, schreibgeschützt. |

### <a name="relationships"></a>Beziehungen
Keine


### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->