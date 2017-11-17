# domainDnsUnavailableRecord-Ressourcentyp
<a id="domaindnsunavailablerecord-resource-type" class="xliff"></a>

Wenn Sie die Navigationseigenschaft **serviceConfigurationRecords** für eine [Domain](domain.md)-Entität abfragen, werden möglicherweise eine oder mehrere [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und/oder [DomainDnsTxtRecord](domaindnstxtrecord.md)-Entitäten zurückgegeben. Diese Entitäten geben die DNS-Einträge an, die Sie der Zonendatei der Domäne hinzufügen müssen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Wenn es nicht möglich ist, solche Entitäten zu generieren, wird stattdessen eine DomainDnsUnavailableRecord-Entität zurückgegeben. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).

## Methoden
<a id="methods" class="xliff"></a>
Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).

## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Gibt den Grund an, warum die **DomainDnsUnavailableRecord**-Entität zurückgegeben wird. |

## Beziehungen
<a id="relationships" class="xliff"></a>
Keine

## JSON-Darstellung
<a id="json-representation" class="xliff"></a>
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->