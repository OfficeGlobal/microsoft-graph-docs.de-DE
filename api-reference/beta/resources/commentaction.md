---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
ms.openlocfilehash: 92dc26945cd591de2ba107907a593159f1e128c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065829"
---
# <a name="commentaction-resource-type"></a>CommentAction-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **CommentAction**-Ressource enthält Informationen zu einer für ein Element vorgenommenen [Kommentaraktivität][].

[Kommentaraktivität]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname    | Typ                       | Beschreibung
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | Wenn der Wert true ist, war die Aktivität eine Antwort auf einen vorhandenen Kommentar-Thread.
| parentAuthor     | [identitySet][]            | Die Identität des Benutzers, der den Kommentar-Thread gestartet hat.
| participants     | [IdentitySet][]-Sammlung | Die Identitäten der Benutzer, die an diesem Kommentar-Thread teilnehmen.

[identitySet]: identityset.md

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->
