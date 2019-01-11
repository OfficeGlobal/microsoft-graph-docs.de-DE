---
title: iPv6Range-Ressourcentyp
description: IPV6-Bereich
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84d925cc7885dab4b3e87dbd62060894e741f52c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845746"
---
# <a name="ipv6range-resource-type"></a>iPv6Range-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

IPV6-Bereich

Erbt von [ipRange](../resources/intune-mam-iprange.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lowerAddress|Zeichenfolge|Untere IP-Adresse|
|upperAddress|Zeichenfolge|Obere IP-Adresse|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



