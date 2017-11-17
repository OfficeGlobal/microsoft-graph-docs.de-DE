# domainDnsRecord-Ressourcentyp
<a id="domaindnsrecord-resource-type" class="xliff"></a>

Möglicherweise müssen Sie für jede Domäne im Mandanten DNS-Einträge zur DNS-Zonendatei der Domäne hinzufügen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Die **DomainDnsRecord**-Entität wird verwendet, um eine solche DNS-Einträge darzustellen. Basisentität für [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und [DomainDnsSrvRecord](domaindnssrvrecord.md)-Entitäten.

## Methoden
<a id="methods" class="xliff"></a>
Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).

## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.|
|isOptional|Boolean| Wenn „false“, muss dieser Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. |
|label|String| Wert, der beim Konfigurieren des Namens des DNS-Eintrags auf dem DNS-Host verwendet wird. |
|recordType|String| Gibt an, welche Art von DNS-Eintrag diese Entität darstellt.</br></br>Folgende Werte sind möglich: *CName*, *Mx*, *Srv*, *Txt*</br></br>Schlüssel |
|supportedService|String| Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem DNS-Eintrag.</br></br>Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl)) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu. |

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
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->