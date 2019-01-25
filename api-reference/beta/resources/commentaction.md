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
# <a name="commentaction-resource-type"></a><span data-ttu-id="b2d46-102">CommentAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b2d46-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d46-103">Die **CommentAction**-Ressource enthält Informationen zu einer für ein Element vorgenommenen [Kommentaraktivität][].</span><span class="sxs-lookup"><span data-stu-id="b2d46-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[Kommentaraktivität]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b2d46-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2d46-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b2d46-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2d46-106">Properties</span></span>

| <span data-ttu-id="b2d46-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b2d46-107">Property name</span></span>    | <span data-ttu-id="b2d46-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b2d46-108">Type</span></span>                       | <span data-ttu-id="b2d46-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2d46-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b2d46-110">isReply</span><span class="sxs-lookup"><span data-stu-id="b2d46-110">isReply</span></span>          | <span data-ttu-id="b2d46-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b2d46-111">boolean</span></span>                    | <span data-ttu-id="b2d46-112">Wenn der Wert true ist, war die Aktivität eine Antwort auf einen vorhandenen Kommentar-Thread.</span><span class="sxs-lookup"><span data-stu-id="b2d46-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="b2d46-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="b2d46-113">parentAuthor</span></span>     | <span data-ttu-id="b2d46-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b2d46-114">[identitySet][]</span></span>            | <span data-ttu-id="b2d46-115">Die Identität des Benutzers, der den Kommentar-Thread gestartet hat.</span><span class="sxs-lookup"><span data-stu-id="b2d46-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="b2d46-116">participants</span><span class="sxs-lookup"><span data-stu-id="b2d46-116">participants</span></span>     | <span data-ttu-id="b2d46-117">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2d46-117">[identitySet][] collection</span></span> | <span data-ttu-id="b2d46-118">Die Identitäten der Benutzer, die an diesem Kommentar-Thread teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="b2d46-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="b2d46-120">Hinweise</span><span class="sxs-lookup"><span data-stu-id="b2d46-120">Remarks</span></span>

<span data-ttu-id="b2d46-121">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b2d46-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
