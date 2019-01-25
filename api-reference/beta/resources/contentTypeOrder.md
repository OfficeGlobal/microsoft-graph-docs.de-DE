---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 9b92a8234c493ae9b0f396db7010e7bf717d5959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514369"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="7711c-102">ContentTypeOrder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7711c-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7711c-103">Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="7711c-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7711c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7711c-104">JSON representation</span></span>

<span data-ttu-id="7711c-105">Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="7711c-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="7711c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7711c-106">Properties</span></span>

| <span data-ttu-id="7711c-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7711c-107">Property name</span></span> | <span data-ttu-id="7711c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7711c-108">Type</span></span>    | <span data-ttu-id="7711c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7711c-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="7711c-110">**default**</span><span class="sxs-lookup"><span data-stu-id="7711c-110">**default**</span></span>   | <span data-ttu-id="7711c-111">boolean</span><span class="sxs-lookup"><span data-stu-id="7711c-111">boolean</span></span> | <span data-ttu-id="7711c-112">Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.</span><span class="sxs-lookup"><span data-stu-id="7711c-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="7711c-113">**position**</span><span class="sxs-lookup"><span data-stu-id="7711c-113">**position**</span></span>  | <span data-ttu-id="7711c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7711c-114">Int32</span></span>   | <span data-ttu-id="7711c-115">Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="7711c-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentTypeOrder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
