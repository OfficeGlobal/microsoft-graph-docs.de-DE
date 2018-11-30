---
title: patchContentCommand-Ressourcentyp
description: Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.
ms.openlocfilehash: bfbdceeda0294540f701f9fa458030834e7d7850
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017058"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="ca986-103">patchContentCommand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ca986-103">patchContentCommand resource type</span></span>

<span data-ttu-id="ca986-104">Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca986-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca986-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ca986-105">JSON representation</span></span>

<span data-ttu-id="ca986-106">Es folgt eine JSON-Darstellung der Ressource, die im Text der Anforderung [PATCH pages/{id}\`](../api/page-update.md) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="ca986-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="ca986-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ca986-107">Properties</span></span>
| <span data-ttu-id="ca986-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca986-108">Property</span></span>     | <span data-ttu-id="ca986-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ca986-109">Type</span></span>   |<span data-ttu-id="ca986-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca986-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca986-111">Aktion</span><span class="sxs-lookup"><span data-stu-id="ca986-111">action</span></span>|<span data-ttu-id="ca986-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="ca986-112">onenotePatchActionType</span></span>|<span data-ttu-id="ca986-113">Die auf das Zielelement anzuwendende Aktion.</span><span class="sxs-lookup"><span data-stu-id="ca986-113">The action to perform on the target element.</span></span> <span data-ttu-id="ca986-114">Die möglichen Werte sind: `replace`, `append`, `delete`, `insert`, oder `prepend`.</span><span class="sxs-lookup"><span data-stu-id="ca986-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="ca986-115">content</span><span class="sxs-lookup"><span data-stu-id="ca986-115">content</span></span>|<span data-ttu-id="ca986-116">String</span><span class="sxs-lookup"><span data-stu-id="ca986-116">String</span></span>|<span data-ttu-id="ca986-p102">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` mit der Komponente „Commands“ gesendet werden </span><span class="sxs-lookup"><span data-stu-id="ca986-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="ca986-119">position</span><span class="sxs-lookup"><span data-stu-id="ca986-119">position</span></span>|<span data-ttu-id="ca986-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="ca986-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="ca986-121">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement.</span><span class="sxs-lookup"><span data-stu-id="ca986-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="ca986-122">Die möglichen Werte sind: `after` (Standard) oder `before`.</span><span class="sxs-lookup"><span data-stu-id="ca986-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="ca986-123">target</span><span class="sxs-lookup"><span data-stu-id="ca986-123">target</span></span>|<span data-ttu-id="ca986-124">String</span><span class="sxs-lookup"><span data-stu-id="ca986-124">String</span></span>|<span data-ttu-id="ca986-p104">Das zu aktualisierende Element. Muss die `#<data-id>` oder die generierte `<id>` des Elements oder das Schlüsselwort `body` oder `title` sein.</span><span class="sxs-lookup"><span data-stu-id="ca986-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
