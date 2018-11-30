---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: 8cb47837d8df1c38ed25fc87d3b4d7da450fed1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016222"
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder-Ressourcentyp

Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ    | Beschreibung
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.
| **position**  | Int32   | Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
