---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: 8cb47837d8df1c38ed25fc87d3b4d7da450fed1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016222"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="e9486-102">ContentTypeOrder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e9486-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="e9486-103">Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e9486-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9486-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9486-104">JSON representation</span></span>

<span data-ttu-id="e9486-105">Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9486-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="e9486-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9486-106">Properties</span></span>

| <span data-ttu-id="e9486-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="e9486-107">Property name</span></span> | <span data-ttu-id="e9486-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e9486-108">Type</span></span>    | <span data-ttu-id="e9486-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9486-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="e9486-110">**default**</span><span class="sxs-lookup"><span data-stu-id="e9486-110">**default**</span></span>   | <span data-ttu-id="e9486-111">boolean</span><span class="sxs-lookup"><span data-stu-id="e9486-111">boolean</span></span> | <span data-ttu-id="e9486-112">Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.</span><span class="sxs-lookup"><span data-stu-id="e9486-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="e9486-113">**position**</span><span class="sxs-lookup"><span data-stu-id="e9486-113">**position**</span></span>  | <span data-ttu-id="e9486-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e9486-114">Int32</span></span>   | <span data-ttu-id="e9486-115">Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e9486-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
