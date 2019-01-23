---
title: proxiedDomain-Ressourcentyp
description: Beschreibt die ProxiedDomain Ressource die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b13e880508c80a009eacb520452c66e7b733ad86
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421844"
---
# <a name="proxieddomain-resource-type"></a>proxiedDomain-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Proxydomäne

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ipAddressOrFQDN|Zeichenfolge|Die IP-Adresse oder vollqualifizierten Domänennamen (FQDN).|
|Proxy|Zeichenfolge|Proxy-IP-Adresse oder FQDN.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



