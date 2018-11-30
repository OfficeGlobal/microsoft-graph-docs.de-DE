---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
ms.openlocfilehash: ef816d027f015155cc09195c359523c83589725e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016408"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="bd988-103">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="bd988-103">teamFunSettings resource type</span></span>



<span data-ttu-id="bd988-104">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="bd988-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bd988-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd988-105">Properties</span></span>
| <span data-ttu-id="bd988-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd988-106">Property</span></span>     | <span data-ttu-id="bd988-107">Typ</span><span class="sxs-lookup"><span data-stu-id="bd988-107">Type</span></span>   |<span data-ttu-id="bd988-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd988-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd988-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="bd988-109">allowGiphy</span></span>|<span data-ttu-id="bd988-110">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd988-110">Boolean</span></span>|<span data-ttu-id="bd988-111">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="bd988-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="bd988-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="bd988-112">giphyContentRating</span></span>|<span data-ttu-id="bd988-113">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="bd988-113">String (enum)</span></span>|<span data-ttu-id="bd988-114">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="bd988-114">Giphy content rating.</span></span> <span data-ttu-id="bd988-115">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="bd988-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="bd988-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="bd988-116">allowStickersAndMemes</span></span>|<span data-ttu-id="bd988-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd988-117">Boolean</span></span>|<span data-ttu-id="bd988-118">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="bd988-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="bd988-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="bd988-119">allowCustomMemes</span></span>|<span data-ttu-id="bd988-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd988-120">Boolean</span></span>|<span data-ttu-id="bd988-121">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="bd988-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd988-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd988-122">JSON representation</span></span>

<span data-ttu-id="bd988-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd988-123">The following is a JSON representation of the resource.</span></span>

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
