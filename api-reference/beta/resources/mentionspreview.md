---
title: Ressourcentyp mentionsPreview
description: Stellt Informationen zu Objekten in einer Ressourceninstanz einer Erwähnung dar.
ms.openlocfilehash: cf6bed3cdfb2d3f541438da0c06fcf8f4873c17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064764"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="66ae5-103">Ressourcentyp mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="66ae5-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="66ae5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66ae5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66ae5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66ae5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66ae5-106">Stellt Informationen zu Objekten in einer Ressourceninstanz einer [erwähnen](../resources/mention.md) .</span><span class="sxs-lookup"><span data-stu-id="66ae5-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="66ae5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66ae5-107">Properties</span></span>
| <span data-ttu-id="66ae5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66ae5-108">Property</span></span>     | <span data-ttu-id="66ae5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="66ae5-109">Type</span></span>   |<span data-ttu-id="66ae5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66ae5-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66ae5-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="66ae5-111">isMentioned</span></span> | <span data-ttu-id="66ae5-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="66ae5-112">Boolean</span></span> | <span data-ttu-id="66ae5-113">True, wenn die angemeldeten Benutzers in der Instanz des übergeordneten Ressource genannt wird.</span><span class="sxs-lookup"><span data-stu-id="66ae5-113">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="66ae5-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="66ae5-114">Read-only.</span></span> <span data-ttu-id="66ae5-115">Filter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66ae5-115">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66ae5-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66ae5-116">JSON representation</span></span>

<span data-ttu-id="66ae5-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66ae5-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
