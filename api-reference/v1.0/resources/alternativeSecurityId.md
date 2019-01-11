---
title: alternativeSecurityId-Ressourcentyp
description: Nur für internen Gebrauch.
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853802"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId-Ressourcentyp

Nur für internen Gebrauch.

## <a name="json-representation"></a>JSON-Darstellung

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a>Eigenschaften
| Eigenschaft         | Typ       | Beschreibung
|:-----------------|:-----------|:---------------------
| Typ             | Int32      | Nur zur internen Verwendung
| identityProvider | string     | Nur zur internen Verwendung
| Key              | Edm.Binary | Nur zur internen Verwendung
