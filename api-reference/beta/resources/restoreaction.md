---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
ms.openlocfilehash: ce8f964b336f648cd1432532eb85a69629eb2207
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063535"
---
# <a name="restoreaction-resource-type"></a>RestoreAction-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wenn die **RestoreAction**-Ressource für ein [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element erneut gespeichert hat.

**Hinweis**: Diese Ressource ist heute zwar leer, in künftigen API-Überarbeitungen wird die Ressource aber möglicherweise mit weiteren Eigenschaften gefüllt.

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a>Eigenschaften

Keine. Dieses Facet ist ein NULL- oder Nicht-NULL-Wert und enthält keine Eigenschaften.

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction"
} -->
