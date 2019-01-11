---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
localization_priority: Normal
ms.openlocfilehash: c53d3215e5f515361c66fe2d3d0ad10a5338e0c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852066"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="03f6c-103">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="03f6c-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="03f6c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03f6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03f6c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03f6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03f6c-106">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="03f6c-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="03f6c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03f6c-107">Properties</span></span>
| <span data-ttu-id="03f6c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03f6c-108">Property</span></span>     | <span data-ttu-id="03f6c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="03f6c-109">Type</span></span>   |<span data-ttu-id="03f6c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03f6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03f6c-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="03f6c-111">allowGiphy</span></span>|<span data-ttu-id="03f6c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="03f6c-112">Boolean</span></span>|<span data-ttu-id="03f6c-113">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="03f6c-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="03f6c-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="03f6c-114">giphyContentRating</span></span>|<span data-ttu-id="03f6c-115">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="03f6c-115">String (enum)</span></span>|<span data-ttu-id="03f6c-116">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="03f6c-116">Giphy content rating.</span></span> <span data-ttu-id="03f6c-117">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="03f6c-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="03f6c-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="03f6c-118">allowStickersAndMemes</span></span>|<span data-ttu-id="03f6c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="03f6c-119">Boolean</span></span>|<span data-ttu-id="03f6c-120">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="03f6c-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="03f6c-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="03f6c-121">allowCustomMemes</span></span>|<span data-ttu-id="03f6c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="03f6c-122">Boolean</span></span>|<span data-ttu-id="03f6c-123">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="03f6c-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03f6c-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03f6c-124">JSON representation</span></span>

<span data-ttu-id="03f6c-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03f6c-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
