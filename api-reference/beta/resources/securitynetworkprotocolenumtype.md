---
title: SecurityNetworkProtocol-Enumeration
description: Mögliche Werte für das Netzwerkprotokoll.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511471"
---
# <a name="securitynetworkprotocol-enum"></a>SecurityNetworkProtocol-Enumeration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mögliche Werte für das Netzwerkprotokoll.

## <a name="members"></a>Elemente

|Member|Wert|Beschreibung|
|:---|:---|:---|
|unknown|-1|Unbekanntes Protokoll.|
|IP|(0)|Internetprotokoll.|
|ICMP|-1| Internet Control Message-Protokoll.|
|IGMP|-2| Internet Group Management Protocol.|
|ggp|-3| Gateway zu Gateway-Protokoll.|
|IPv4|4*| Internetprotokoll, Version 4.|
|TCP|-6| Transmission Control-Protokoll.|
|PUP|1.2| PARC Universal Paket Protokoll.|
|UDP|1.7| User Datagram-Protokoll.|
|IDP|2.2| Internet Datagram-Protokoll.|
|IPv6|4.1| Internetprotokoll, Version 6 (ipv6).|
|ipv6RoutingHeader|4.3| IPv6-Routing-Header.|
|ipv6FragmentHeader|4.4| IPv6-Fragment Header.|
|ipSecEncapsulatingSecurityPayload|50%| IPv6-Encapsulating Security Payload-Header.|
|ipSecAuthenticationHeader|5.1| IPv6-Authentication-Header.|
|icmpV6|5.8| Internet Control Message Protocol für ipv6.|
|ipv6NoNextHeader|5.9| IPv6 keine nächste Kopfzeile.|
|ipv6DestinationOptions|-60| IPv6-Ziel-Optionen-Header.|
|nd|7.7| NET Disk-Protokoll (nicht offizieller).|
|Raw|255| Unformatierte Protokoll für die IP-Pakete.|
|IPX|-1000| Internet Packet Exchange-Protokoll.|
|SPX|1256| Sequenzierten Pakets Exchange-Protokoll.|
|spxII|1257| Sequenzierten Pakets Exchange Version 2-Protokoll.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
