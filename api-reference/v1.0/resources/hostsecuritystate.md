---
title: Ressourcentyp hostSecurityState
description: Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816338"
---
# <a name="hostsecuritystate-resource-type"></a>Ressourcentyp hostSecurityState

Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|FQDN|String|Hosten der FQDN (Fully Qualified Domain Name) (z. B. `machine.company.com`).|
|isAzureAadJoined|Boolean|True, wenn der Host Domäne Azure Active Directory Domain Services beigetreten ist.|
|isAzureAadRegistered|Boolean|True, wenn der Host mit Azure Active Directory Gerät-Registrierung (BYOD Geräte - d. h., nicht vollständig durch Enterprise verwaltet) registriert.|
|isHybridAzureDomainJoined|Boolean|True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.|
|netBiosName|String|Der Name der lokalen Host ohne den DNS-Domänennamen.|
|Betriebssystem|String|Host-Betriebssystem. (Z. B. Windows10, Mac OS, RHEL, usw.).|
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
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
