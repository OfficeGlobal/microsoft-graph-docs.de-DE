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
# <a name="commentaction-resource-type"></a><span data-ttu-id="df9b1-102">CommentAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df9b1-102">CommentAction resource type</span></span>

> <span data-ttu-id="df9b1-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df9b1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df9b1-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df9b1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df9b1-105">Die **CommentAction**-Ressource enthält Informationen zu einer für ein Element vorgenommenen [Kommentaraktivität][].</span><span class="sxs-lookup"><span data-stu-id="df9b1-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[Kommentaraktivität]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="df9b1-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df9b1-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="df9b1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df9b1-108">Properties</span></span>

| <span data-ttu-id="df9b1-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="df9b1-109">Property name</span></span>    | <span data-ttu-id="df9b1-110">Typ</span><span class="sxs-lookup"><span data-stu-id="df9b1-110">Type</span></span>                       | <span data-ttu-id="df9b1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df9b1-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="df9b1-112">isReply</span><span class="sxs-lookup"><span data-stu-id="df9b1-112">isReply</span></span>          | <span data-ttu-id="df9b1-113">boolean</span><span class="sxs-lookup"><span data-stu-id="df9b1-113">boolean</span></span>                    | <span data-ttu-id="df9b1-114">Wenn der Wert true ist, war die Aktivität eine Antwort auf einen vorhandenen Kommentar-Thread.</span><span class="sxs-lookup"><span data-stu-id="df9b1-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="df9b1-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="df9b1-115">parentAuthor</span></span>     | <span data-ttu-id="df9b1-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df9b1-116">[identitySet][]</span></span>            | <span data-ttu-id="df9b1-117">Die Identität des Benutzers, der den Kommentar-Thread gestartet hat.</span><span class="sxs-lookup"><span data-stu-id="df9b1-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="df9b1-118">participants</span><span class="sxs-lookup"><span data-stu-id="df9b1-118">participants</span></span>     | <span data-ttu-id="df9b1-119">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="df9b1-119">[identitySet][] collection</span></span> | <span data-ttu-id="df9b1-120">Die Identitäten der Benutzer, die an diesem Kommentar-Thread teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="df9b1-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="df9b1-122">Hinweise</span><span class="sxs-lookup"><span data-stu-id="df9b1-122">Remarks</span></span>

<span data-ttu-id="df9b1-123">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="df9b1-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->
