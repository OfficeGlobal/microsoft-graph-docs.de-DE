---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Stamm
ms.openlocfilehash: 771eb39baf2a7ce7a85fb43120d6e9e7358f6f6c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061879"
---
# <a name="root-resource-type"></a>Root-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Das **Root**-Facet gibt an, dass ein Objekt in der Hierarchie an der obersten Stelle steht.
Das Vorhandensein (Nicht-NULL) des Facetwerts gibt an, dass das Objekt der Stamm ist.
Ein Nullwert (oder ein fehlender Wert) bedeutet, dass das Objekt nicht der Stamm ist.

**Hinweis**: Dieses Facet ist heute zwar leer, in künftigen API-Überarbeitungen wird das Facet aber möglicherweise mit weiteren Eigenschaften gefüllt.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>Eigenschaften

Die **root**-Ressource hat keine Eigenschaften.


<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root"
} -->
