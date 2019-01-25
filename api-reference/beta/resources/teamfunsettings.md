---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515860"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="972a5-103">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="972a5-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="972a5-104">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="972a5-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="972a5-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="972a5-105">Properties</span></span>
| <span data-ttu-id="972a5-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="972a5-106">Property</span></span>     | <span data-ttu-id="972a5-107">Typ</span><span class="sxs-lookup"><span data-stu-id="972a5-107">Type</span></span>   |<span data-ttu-id="972a5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="972a5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="972a5-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="972a5-109">allowGiphy</span></span>|<span data-ttu-id="972a5-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="972a5-110">Boolean</span></span>|<span data-ttu-id="972a5-111">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="972a5-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="972a5-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="972a5-112">giphyContentRating</span></span>|<span data-ttu-id="972a5-113">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="972a5-113">String (enum)</span></span>|<span data-ttu-id="972a5-114">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="972a5-114">Giphy content rating.</span></span> <span data-ttu-id="972a5-115">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="972a5-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="972a5-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="972a5-116">allowStickersAndMemes</span></span>|<span data-ttu-id="972a5-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="972a5-117">Boolean</span></span>|<span data-ttu-id="972a5-118">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="972a5-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="972a5-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="972a5-119">allowCustomMemes</span></span>|<span data-ttu-id="972a5-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="972a5-120">Boolean</span></span>|<span data-ttu-id="972a5-121">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="972a5-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="972a5-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="972a5-122">JSON representation</span></span>

<span data-ttu-id="972a5-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="972a5-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
