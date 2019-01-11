---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ccea5804c3f4eddb02b5d4163302362f29b5fbc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890496"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="66e25-102">ContentTypeOrder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="66e25-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="66e25-103">Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="66e25-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66e25-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66e25-104">JSON representation</span></span>

<span data-ttu-id="66e25-105">Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="66e25-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="66e25-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66e25-106">Properties</span></span>

| <span data-ttu-id="66e25-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="66e25-107">Property name</span></span> | <span data-ttu-id="66e25-108">Typ</span><span class="sxs-lookup"><span data-stu-id="66e25-108">Type</span></span>    | <span data-ttu-id="66e25-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66e25-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="66e25-110">**default**</span><span class="sxs-lookup"><span data-stu-id="66e25-110">**default**</span></span>   | <span data-ttu-id="66e25-111">boolean</span><span class="sxs-lookup"><span data-stu-id="66e25-111">boolean</span></span> | <span data-ttu-id="66e25-112">Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.</span><span class="sxs-lookup"><span data-stu-id="66e25-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="66e25-113">**position**</span><span class="sxs-lookup"><span data-stu-id="66e25-113">**position**</span></span>  | <span data-ttu-id="66e25-114">Int32</span><span class="sxs-lookup"><span data-stu-id="66e25-114">Int32</span></span>   | <span data-ttu-id="66e25-115">Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="66e25-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
