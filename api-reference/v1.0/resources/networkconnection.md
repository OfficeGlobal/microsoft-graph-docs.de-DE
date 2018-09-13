# <a name="networkconnection-resource-type"></a>networkConnection-Ressourcentyp

Enthält zustandsbehaftete Informationen zur Netzwerkverbindung, die sich auf die Warnung beziehen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|applicationName|Zeichenfolge|Name der Anwendung, die die Netzwerkverbindung verwaltet (z. B. Facebook, SMTP usw.).|
|destinationAddress|Zeichenfolge|Ziel-IP-Adresse (der Netzwerkverbindung).|
|destinationDomain|Zeichenfolge|Zieldomänenteil der Ziel-URL. (zum Beispiel "www.contoso.com").|
|destinationPort|Zeichenfolge|Zielport (der Netzwerkverbindung).|
|destinationUrl|Zeichenfolge|Netzwerkverbindungs-URL / URI-Zeichenfolge - ohne Parameter. (zum Beispiel "www.contoso.com/products/default.html")|
|Richtung|connectionDirection|Richtung der Netzwerkverbindung. Mögliche Werte sind: `unknown`, `inbound` und `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Datum, an dem die Zieldomäne registriert wurde. Der Zeitstempel-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|localDnsName|Zeichenfolge|Die lokale DNS-Namensauflösung, die im lokalen DNS-Cache des Hosts angezeigt wird (z. B. für den Fall, dass die Datei "hosts" manipuliert wurde).|
|natDestinationAddress|Zeichenfolge|Netzwerkadressenübersetzung Ziel-IP-Adresse.|
|natDestinationPort|Zeichenfolge|Netzwerkadressenübersetzung Zielport.|
|natSourceAddress|Zeichenfolge|Netzwerkadressenübersetzung Ursprungs-IP-Adresse.|
|natSourcePort|Zeichenfolge|Netzwerkadressenübersetzung Quellport.|
|Protokoll|[securityNetworkProtocol](securitynetworkprotocol.md)|Netzwerkprotokoll Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|Zeichenfolge|Vom Provider generierte / berechnete Risikobewertung der Netzwerkverbindung. Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.|
|SourceAddress|Zeichenfolge|Quell- (d. h. Ursprung) IP-Adresse (der Netzwerkverbindung).|
|sourcePort|Zeichenfolge|Quelle (d. h. Ursprung) IP-Port (der Netzwerkverbindung).|
|Status|connectionStatus|Status der Netzwerkverbinung Mögliche Werte: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Zeichenfolge|Parameter (Suffix) der Ziel-URL.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->