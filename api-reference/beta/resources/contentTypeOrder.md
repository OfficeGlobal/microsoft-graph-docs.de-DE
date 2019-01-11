---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ad25ececa9a32a1aaab7f25bf909f7e1ef640dec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825753"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="d898e-102">ContentTypeOrder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d898e-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="d898e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d898e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d898e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d898e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d898e-105">Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d898e-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d898e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d898e-106">JSON representation</span></span>

<span data-ttu-id="d898e-107">Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d898e-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="d898e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d898e-108">Properties</span></span>

| <span data-ttu-id="d898e-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d898e-109">Property name</span></span> | <span data-ttu-id="d898e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d898e-110">Type</span></span>    | <span data-ttu-id="d898e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d898e-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="d898e-112">**default**</span><span class="sxs-lookup"><span data-stu-id="d898e-112">**default**</span></span>   | <span data-ttu-id="d898e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="d898e-113">boolean</span></span> | <span data-ttu-id="d898e-114">Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.</span><span class="sxs-lookup"><span data-stu-id="d898e-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="d898e-115">**position**</span><span class="sxs-lookup"><span data-stu-id="d898e-115">**position**</span></span>  | <span data-ttu-id="d898e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d898e-116">Int32</span></span>   | <span data-ttu-id="d898e-117">Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d898e-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
