---
title: NetworkConnection Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 6d28149854ed3157473b678db442ee3474e456c6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571919"
---
# <a name="networkconnection-resource-type"></a>NetworkConnection Ressourcentyp

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|applicationName|String|Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).|
|destinationAddress|String|Ziel-IP-Adresse (der Verbindung).|
|destinationDomain|String|Ziel der Domänenteil der Ziel-URL. (zum Beispiel "www.contoso.com").|
|destinationPort|String|Zielport (der Verbindung).|
|destinationUrl|String|Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen. (zum Beispiel "www.contoso.com/products/default.html")|
|Richtung|connectionDirection|Richtung der Netzwerk-Verbindung. Mögliche Werte sind: `unknown`, `inbound` und `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Datum, wenn die Zieldomäne registriert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|localDnsName|String|Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).|
|natDestinationAddress|String|Network Address Translation Ziel-IP-Adresse.|
|natDestinationPort|String|Network Address Translation Zielport.|
|natSourceAddress|String|Network Address Translation Quell-IP-Adresse.|
|natSourcePort|String|Network Address Translation Quellport.|
|protocol| securityNetworkProtocol |Netzwerkprotokoll. Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|String|Anbieter generiert/berechnet riskieren Bewertung der Verbindung. Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.|
|sourceAddress|String|Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).|
|Quellport|String|Quelle (d. h. Ursprung) IP-Port (der Verbindung).|
|status|connectionStatus|Netzwerk-Verbindungsstatus. Mögliche Werte sind: `unknown`, `attempted`, `succeeded`, `blocked` und `failed`.|
|urlParameters|String|Parameter (Suffix) der Ziel-URL.|

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
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
