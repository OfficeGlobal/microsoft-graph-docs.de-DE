---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
ms.openlocfilehash: be873ba2b5f9bc1fdd387407c1036435dc6f1fc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061262"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="61289-102">MentionAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61289-102">MentionAction resource type</span></span>

> <span data-ttu-id="61289-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61289-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61289-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61289-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61289-105">Die **MentionAction**-Ressource enthält Informationen zu einer [Aktivität][], in der Personen erwähnt wurden.</span><span class="sxs-lookup"><span data-stu-id="61289-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[Aktivität]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="61289-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61289-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="61289-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61289-108">Properties</span></span>

| <span data-ttu-id="61289-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="61289-109">Property name</span></span> | <span data-ttu-id="61289-110">Typ</span><span class="sxs-lookup"><span data-stu-id="61289-110">Type</span></span>                       | <span data-ttu-id="61289-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61289-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="61289-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="61289-112">mentionees</span></span>    | <span data-ttu-id="61289-113">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="61289-113">[identitySet][] collection</span></span> | <span data-ttu-id="61289-114">Die Identität der in dieser Aktion erwähnten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="61289-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="61289-116">Hinweise</span><span class="sxs-lookup"><span data-stu-id="61289-116">Remarks</span></span>

<span data-ttu-id="61289-117">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="61289-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
