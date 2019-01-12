---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ac49c80a39fd6bc51b048a8eb7dab6e62da810
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974140"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="12ae3-102">MentionAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="12ae3-102">MentionAction resource type</span></span>

> <span data-ttu-id="12ae3-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12ae3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12ae3-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12ae3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12ae3-105">Die **MentionAction**-Ressource enthält Informationen zu einer [Aktivität][], in der Personen erwähnt wurden.</span><span class="sxs-lookup"><span data-stu-id="12ae3-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[Aktivität]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="12ae3-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12ae3-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="12ae3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12ae3-108">Properties</span></span>

| <span data-ttu-id="12ae3-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="12ae3-109">Property name</span></span> | <span data-ttu-id="12ae3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="12ae3-110">Type</span></span>                       | <span data-ttu-id="12ae3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12ae3-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="12ae3-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="12ae3-112">mentionees</span></span>    | <span data-ttu-id="12ae3-113">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="12ae3-113">[identitySet][] collection</span></span> | <span data-ttu-id="12ae3-114">Die Identität der in dieser Aktion erwähnten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="12ae3-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="12ae3-116">Hinweise</span><span class="sxs-lookup"><span data-stu-id="12ae3-116">Remarks</span></span>

<span data-ttu-id="12ae3-117">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="12ae3-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
