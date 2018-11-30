---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="b1d9d-102">ContentTypeOrder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b1d9d-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="b1d9d-103">Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1d9d-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1d9d-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b1d9d-104">JSON representation</span></span>

<span data-ttu-id="b1d9d-105">Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="b1d9d-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="b1d9d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b1d9d-106">Properties</span></span>

| <span data-ttu-id="b1d9d-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b1d9d-107">Property name</span></span> | <span data-ttu-id="b1d9d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b1d9d-108">Type</span></span>    | <span data-ttu-id="b1d9d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1d9d-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="b1d9d-110">**default**</span><span class="sxs-lookup"><span data-stu-id="b1d9d-110">**default**</span></span>   | <span data-ttu-id="b1d9d-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b1d9d-111">boolean</span></span> | <span data-ttu-id="b1d9d-112">Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.</span><span class="sxs-lookup"><span data-stu-id="b1d9d-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="b1d9d-113">**position**</span><span class="sxs-lookup"><span data-stu-id="b1d9d-113">**position**</span></span>  | <span data-ttu-id="b1d9d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d9d-114">Int32</span></span>   | <span data-ttu-id="b1d9d-115">Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b1d9d-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
