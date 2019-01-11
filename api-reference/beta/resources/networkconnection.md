---
title: NetworkConnection Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: a20520a729076c7e63079c6dfc803659ace45b9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880059"
---
# <a name="networkconnection-resource-type"></a>NetworkConnection Ressourcentyp

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|applicationName|String|Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).|
|destinationAddress|Zeichenfolge|Ziel-IP-Adresse (der Verbindung).|
|destinationDomain|Zeichenfolge|Ziel der Domänenteil der Ziel-URL. (zum Beispiel "www.contoso.com").|
|destinationPort|Zeichenfolge|Zielport (der Verbindung).|
|destinationUrl|Zeichenfolge|Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen. (zum Beispiel "www.contoso.com/products/default.html")|
|Richtung|connectionDirection|Richtung der Netzwerk-Verbindung. Mögliche Werte sind: `unknown`, `inbound` und `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Datum, wenn die Zieldomäne registriert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|localDnsName|Zeichenfolge|Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).|
|natDestinationAddress|Zeichenfolge|Network Address Translation Ziel-IP-Adresse.|
|natDestinationPort|Zeichenfolge|Network Address Translation Zielport.|
|natSourceAddress|Zeichenfolge|Network Address Translation Quell-IP-Adresse.|
|natSourcePort|Zeichenfolge|Network Address Translation Quellport.|
|protocol|[securityNetworkProtocol](securitynetworkprotocolenumtype.md)|Netzwerkprotokoll. Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|Zeichenfolge|Anbieter generiert/berechnet riskieren Bewertung der Verbindung. Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.|
|sourceAddress|Zeichenfolge|Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).|
|Quellport|Zeichenfolge|Quelle (d. h. Ursprung) IP-Port (der Verbindung).|
|status|connectionStatus|Netzwerk-Verbindungsstatus. Mögliche Werte sind: `unknown`, `attempted`, `succeeded`, `blocked` und `failed`.|
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
