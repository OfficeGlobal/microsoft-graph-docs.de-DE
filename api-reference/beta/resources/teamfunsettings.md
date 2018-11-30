---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
ms.openlocfilehash: e8cf62b88a3afa3e5caf6b9425312d7a26af4d20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058554"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="aa6f7-103">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="aa6f7-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="aa6f7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa6f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa6f7-106">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="aa6f7-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aa6f7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa6f7-107">Properties</span></span>
| <span data-ttu-id="aa6f7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa6f7-108">Property</span></span>     | <span data-ttu-id="aa6f7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="aa6f7-109">Type</span></span>   |<span data-ttu-id="aa6f7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa6f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6f7-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="aa6f7-111">allowGiphy</span></span>|<span data-ttu-id="aa6f7-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa6f7-112">Boolean</span></span>|<span data-ttu-id="aa6f7-113">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="aa6f7-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="aa6f7-114">giphyContentRating</span></span>|<span data-ttu-id="aa6f7-115">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="aa6f7-115">String (enum)</span></span>|<span data-ttu-id="aa6f7-116">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-116">Giphy content rating.</span></span> <span data-ttu-id="aa6f7-117">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="aa6f7-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="aa6f7-118">allowStickersAndMemes</span></span>|<span data-ttu-id="aa6f7-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa6f7-119">Boolean</span></span>|<span data-ttu-id="aa6f7-120">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="aa6f7-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="aa6f7-121">allowCustomMemes</span></span>|<span data-ttu-id="aa6f7-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa6f7-122">Boolean</span></span>|<span data-ttu-id="aa6f7-123">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa6f7-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa6f7-124">JSON representation</span></span>

<span data-ttu-id="aa6f7-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa6f7-125">The following is a JSON representation of the resource.</span></span>

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
