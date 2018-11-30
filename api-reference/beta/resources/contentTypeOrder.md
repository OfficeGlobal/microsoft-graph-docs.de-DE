---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: a6b83627d86bbb35357f03dbee3605c6fb1df7a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065116"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="bbe93-102">ContentTypeOrder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bbe93-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="bbe93-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bbe93-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbe93-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bbe93-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbe93-105">Die **ContentTypeOrder**-Ressource gibt an, in welcher Reihenfolge der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="bbe93-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbe93-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bbe93-106">JSON representation</span></span>

<span data-ttu-id="bbe93-107">Es folgt eine JSON-Darstellung einer **contentTypeOrder**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bbe93-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="bbe93-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bbe93-108">Properties</span></span>

| <span data-ttu-id="bbe93-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bbe93-109">Property name</span></span> | <span data-ttu-id="bbe93-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bbe93-110">Type</span></span>    | <span data-ttu-id="bbe93-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbe93-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="bbe93-112">**default**</span><span class="sxs-lookup"><span data-stu-id="bbe93-112">**default**</span></span>   | <span data-ttu-id="bbe93-113">boolean</span><span class="sxs-lookup"><span data-stu-id="bbe93-113">boolean</span></span> | <span data-ttu-id="bbe93-114">Gibt an, ob es sich  um den standardmäßigen Inhaltstyp handelt.</span><span class="sxs-lookup"><span data-stu-id="bbe93-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="bbe93-115">**position**</span><span class="sxs-lookup"><span data-stu-id="bbe93-115">**position**</span></span>  | <span data-ttu-id="bbe93-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bbe93-116">Int32</span></span>   | <span data-ttu-id="bbe93-117">Gibt die Position an, an welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="bbe93-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
