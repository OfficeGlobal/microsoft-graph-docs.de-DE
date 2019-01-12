---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b4c30afb6d0c10e8f011b779cf257a1627ff7b48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949780"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="f7e47-103">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="f7e47-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="f7e47-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7e47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7e47-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7e47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7e47-106">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="f7e47-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f7e47-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7e47-107">Properties</span></span>
| <span data-ttu-id="f7e47-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7e47-108">Property</span></span>     | <span data-ttu-id="f7e47-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f7e47-109">Type</span></span>   |<span data-ttu-id="f7e47-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7e47-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7e47-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="f7e47-111">allowGiphy</span></span>|<span data-ttu-id="f7e47-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f7e47-112">Boolean</span></span>|<span data-ttu-id="f7e47-113">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f7e47-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="f7e47-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="f7e47-114">giphyContentRating</span></span>|<span data-ttu-id="f7e47-115">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="f7e47-115">String (enum)</span></span>|<span data-ttu-id="f7e47-116">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="f7e47-116">Giphy content rating.</span></span> <span data-ttu-id="f7e47-117">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="f7e47-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="f7e47-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="f7e47-118">allowStickersAndMemes</span></span>|<span data-ttu-id="f7e47-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f7e47-119">Boolean</span></span>|<span data-ttu-id="f7e47-120">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="f7e47-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="f7e47-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="f7e47-121">allowCustomMemes</span></span>|<span data-ttu-id="f7e47-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f7e47-122">Boolean</span></span>|<span data-ttu-id="f7e47-123">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f7e47-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7e47-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7e47-124">JSON representation</span></span>

<span data-ttu-id="f7e47-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7e47-125">The following is a JSON representation of the resource.</span></span>

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
