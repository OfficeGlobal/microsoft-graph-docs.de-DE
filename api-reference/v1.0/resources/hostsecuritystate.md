# <a name="hostsecuritystate-resource-type"></a>Ressourcentyp hostSecurityState

Enthält Zustandsinformationen über den Host (einschließlich der Geräte, Computer und usw.).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|fqdn|Zeichenfolge|Host FQDN (Fully Qualified Domain Name) (z.B. `machine.company.com`).|
|isAzureAadJoined|Boolesch|True, wenn der Host Teil der Azure Active Directory Domain Services ist.|
|isAzureAadRegistered|Boolesch|True, wenn der Host mit der Azure Active Directory Gerät-Registrierung (BYOD Geräte - d.h., nicht vollständig durch Enterprise verwaltet) registriert ist.|
|isHybridAzureDomainJoined|Boolesch|True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.|
|netBiosName|Zeichenfolge|Der Name der lokalen Host ohne den DNS-Domänennamen.|
|os|Zeichenfolge|Hostbetriebssystem. (Z.B. Windows10, Mac OS, RHEL, usw.).|
|privateIpAddress|Zeichenfolge|Private (nicht-routingfähige) IPv4- oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.|
|publicIpAddress|Zeichenfolge|Öffentliche routingfähige IPv4- oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.|
|riskScore|Zeichenfolge|Vom Anbieter generierte/berechnete Risikobewertung des Hosts.  Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
