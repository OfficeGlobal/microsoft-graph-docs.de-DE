---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: e674c996002b3a54c92886dd1c5dca7a76c56b51
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526270"
---
# <a name="commentaction-resource-type"></a>CommentAction-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/commentaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
