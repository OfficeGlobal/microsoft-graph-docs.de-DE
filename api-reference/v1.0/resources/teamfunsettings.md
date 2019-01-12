---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987671"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="08cd0-103">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="08cd0-103">teamFunSettings resource type</span></span>



<span data-ttu-id="08cd0-104">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="08cd0-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="08cd0-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08cd0-105">Properties</span></span>
| <span data-ttu-id="08cd0-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08cd0-106">Property</span></span>     | <span data-ttu-id="08cd0-107">Typ</span><span class="sxs-lookup"><span data-stu-id="08cd0-107">Type</span></span>   |<span data-ttu-id="08cd0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08cd0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08cd0-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="08cd0-109">allowGiphy</span></span>|<span data-ttu-id="08cd0-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08cd0-110">Boolean</span></span>|<span data-ttu-id="08cd0-111">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="08cd0-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="08cd0-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="08cd0-112">giphyContentRating</span></span>|<span data-ttu-id="08cd0-113">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="08cd0-113">String (enum)</span></span>|<span data-ttu-id="08cd0-114">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="08cd0-114">Giphy content rating.</span></span> <span data-ttu-id="08cd0-115">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="08cd0-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="08cd0-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="08cd0-116">allowStickersAndMemes</span></span>|<span data-ttu-id="08cd0-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08cd0-117">Boolean</span></span>|<span data-ttu-id="08cd0-118">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="08cd0-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="08cd0-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="08cd0-119">allowCustomMemes</span></span>|<span data-ttu-id="08cd0-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08cd0-120">Boolean</span></span>|<span data-ttu-id="08cd0-121">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="08cd0-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08cd0-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08cd0-122">JSON representation</span></span>

<span data-ttu-id="08cd0-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08cd0-123">The following is a JSON representation of the resource.</span></span>

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
