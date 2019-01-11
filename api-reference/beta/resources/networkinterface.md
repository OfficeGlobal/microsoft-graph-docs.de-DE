---
title: NetworkInterface-Ressourcentyp
description: Stellt eine Network Interface Card (NIC) Hosts zugeordnet.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823303"
---
# <a name="networkinterface-resource-type"></a>NetworkInterface-Ressourcentyp

Stellt eine Network Interface Card (NIC) Hosts zugeordnet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Beschreibung der NIC (z. B. Ethernet-Adapter, WLAN-Adapter LAN-Verbindung * <> # usw..).|
|ipV4Address|String|Letzte IPv4-Adresse zugeordneten dieser Netzwerkkarte|
|ipV6Address|String|Letzte Öffentliche (auch bekannt als global) IPv6-Adresse zugeordneten dieser Netzwerkkarte|
|localIpV6Address|String|Letzte (Link-Local oder Site-Local) IPv6 zugeordnete lokale Adresse diese Netzwerkkarte ein.|
|macAddress|String|MAC-Adresse der Netzwerkkarte auf diesem Host.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
