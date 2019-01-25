---
title: Ressourcentyp hostSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526697"
---
# <a name="hostsecuritystate-resource-type"></a>Ressourcentyp hostSecurityState

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|FQDN|String|Host-FQDN (Fully Qualified Domain Name) (beispielsweise machine.company.com).|
|isAzureAadJoined|Boolescher Wert|True, wenn der Host Domäne Azure Active Directory Domain Services beigetreten ist.|
|isAzureAadRegistered|Boolescher Wert|True, wenn der Host mit Azure Active Directory Gerät-Registrierung (BYOD Geräte - d. h., nicht vollständig durch Enterprise verwaltet) registriert.|
|isHybridAzureDomainJoined|Boolescher Wert|True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.|
|netBiosName|String|Der Name der lokalen Host ohne den DNS-Domänennamen.|
|I-5.|String|Host-Betriebssystem. (Z. B. Windows10, Mac OS, RHEL, usw.).|
|Priv.IP-Adresse|String|Private (nicht-routingfähige) IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.|
|Öffentl.IP|String|Öffentlich routingfähige IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.|
|riskScore|String|Provider-generiert/berechnet Risiko Bewertung des Hosts.  Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.|

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
