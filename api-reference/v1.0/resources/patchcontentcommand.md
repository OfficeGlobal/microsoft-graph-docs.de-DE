---
title: patchContentCommand-Ressourcentyp
description: Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.
localization_priority: Normal
ms.openlocfilehash: fb0900490b3fe05e6fb90dc4ab8252620bf43983
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804536"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="bf2e2-103">patchContentCommand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bf2e2-103">patchContentCommand resource type</span></span>

<span data-ttu-id="bf2e2-104">Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf2e2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bf2e2-105">JSON representation</span></span>

<span data-ttu-id="bf2e2-106">Es folgt eine JSON-Darstellung der Ressource, die im Text der Anforderung [PATCH pages/{id}\`](../api/page-update.md) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="bf2e2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bf2e2-107">Properties</span></span>
| <span data-ttu-id="bf2e2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf2e2-108">Property</span></span>     | <span data-ttu-id="bf2e2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bf2e2-109">Type</span></span>   |<span data-ttu-id="bf2e2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf2e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2e2-111">Aktion</span><span class="sxs-lookup"><span data-stu-id="bf2e2-111">action</span></span>|<span data-ttu-id="bf2e2-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="bf2e2-112">onenotePatchActionType</span></span>|<span data-ttu-id="bf2e2-113">Die auf das Zielelement anzuwendende Aktion.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-113">The action to perform on the target element.</span></span> <span data-ttu-id="bf2e2-114">Die möglichen Werte sind: `replace`, `append`, `delete`, `insert`, oder `prepend`.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="bf2e2-115">content</span><span class="sxs-lookup"><span data-stu-id="bf2e2-115">content</span></span>|<span data-ttu-id="bf2e2-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bf2e2-116">String</span></span>|<span data-ttu-id="bf2e2-p102">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` mit der Komponente „Commands“ gesendet werden </span><span class="sxs-lookup"><span data-stu-id="bf2e2-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="bf2e2-119">position</span><span class="sxs-lookup"><span data-stu-id="bf2e2-119">position</span></span>|<span data-ttu-id="bf2e2-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="bf2e2-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="bf2e2-121">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="bf2e2-122">Die möglichen Werte sind: `after` (Standard) oder `before`.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="bf2e2-123">target</span><span class="sxs-lookup"><span data-stu-id="bf2e2-123">target</span></span>|<span data-ttu-id="bf2e2-124">String</span><span class="sxs-lookup"><span data-stu-id="bf2e2-124">String</span></span>|<span data-ttu-id="bf2e2-p104">Das zu aktualisierende Element. Muss die `#<data-id>` oder die generierte `<id>` des Elements oder das Schlüsselwort `body` oder `title` sein.</span><span class="sxs-lookup"><span data-stu-id="bf2e2-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
