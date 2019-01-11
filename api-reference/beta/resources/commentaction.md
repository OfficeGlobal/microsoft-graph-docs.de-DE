---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: 952a86161047ab869238feaba50b8ad4d8ce0658
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845598"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="64369-102">CommentAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="64369-102">CommentAction resource type</span></span>

> <span data-ttu-id="64369-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="64369-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64369-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64369-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64369-105">Die **CommentAction**-Ressource enthält Informationen zu einer für ein Element vorgenommenen [Kommentaraktivität][].</span><span class="sxs-lookup"><span data-stu-id="64369-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[Kommentaraktivität]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="64369-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64369-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="64369-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64369-108">Properties</span></span>

| <span data-ttu-id="64369-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="64369-109">Property name</span></span>    | <span data-ttu-id="64369-110">Typ</span><span class="sxs-lookup"><span data-stu-id="64369-110">Type</span></span>                       | <span data-ttu-id="64369-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64369-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="64369-112">isReply</span><span class="sxs-lookup"><span data-stu-id="64369-112">isReply</span></span>          | <span data-ttu-id="64369-113">boolean</span><span class="sxs-lookup"><span data-stu-id="64369-113">boolean</span></span>                    | <span data-ttu-id="64369-114">Wenn der Wert true ist, war die Aktivität eine Antwort auf einen vorhandenen Kommentar-Thread.</span><span class="sxs-lookup"><span data-stu-id="64369-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="64369-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="64369-115">parentAuthor</span></span>     | <span data-ttu-id="64369-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="64369-116">[identitySet][]</span></span>            | <span data-ttu-id="64369-117">Die Identität des Benutzers, der den Kommentar-Thread gestartet hat.</span><span class="sxs-lookup"><span data-stu-id="64369-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="64369-118">participants</span><span class="sxs-lookup"><span data-stu-id="64369-118">participants</span></span>     | <span data-ttu-id="64369-119">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="64369-119">[identitySet][] collection</span></span> | <span data-ttu-id="64369-120">Die Identitäten der Benutzer, die an diesem Kommentar-Thread teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="64369-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="64369-122">Hinweise</span><span class="sxs-lookup"><span data-stu-id="64369-122">Remarks</span></span>

<span data-ttu-id="64369-123">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="64369-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->
