# <a name="domaindnsmxrecord-resource-type"></a>domainDnsMxRecord-Ressourcentyp

Stellt einen MX-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).

### <a name="methods"></a>Methoden
Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).

### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.|
|isOptional|Boolean| Wenn „false“, muss der MX-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. |
|label|String| Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird. |
|mailExchange|String| Wert, der beim Konfigurieren der *answer/destination/value*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.|
|preference|Int32| Wert, der beim Konfigurieren der *Preference/Priority*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird. |
|recordType|String| Typ des DNS-Eintrags. Der Wert ist immer *MX*. Schlüssel |
|supportedService|String| Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem MX-Eintrag.</br></br>Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu. |

### <a name="relationships"></a>Beziehungen
Keine

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->