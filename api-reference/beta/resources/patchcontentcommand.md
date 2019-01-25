---
title: patchContentCommand-Ressourcentyp
description: Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523883"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="487dd-103">patchContentCommand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="487dd-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="487dd-104">Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="487dd-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="487dd-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="487dd-105">JSON representation</span></span>

<span data-ttu-id="487dd-106">Es folgt eine JSON-Darstellung der Ressource, die im Text der Anforderung [PATCH pages/{id}\`](../api/page-update.md) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="487dd-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="487dd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="487dd-107">Properties</span></span>
| <span data-ttu-id="487dd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="487dd-108">Property</span></span>     | <span data-ttu-id="487dd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="487dd-109">Type</span></span>   |<span data-ttu-id="487dd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="487dd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="487dd-111">action</span><span class="sxs-lookup"><span data-stu-id="487dd-111">action</span></span>|<span data-ttu-id="487dd-112">String</span><span class="sxs-lookup"><span data-stu-id="487dd-112">String</span></span>|<span data-ttu-id="487dd-p101">Die für das Zielelement auszuführende Aktion. Mögliche Werte sind: `replace`, `append`, `delete`, `insert` oder `prepend`.</span><span class="sxs-lookup"><span data-stu-id="487dd-p101">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="487dd-115">content</span><span class="sxs-lookup"><span data-stu-id="487dd-115">content</span></span>|<span data-ttu-id="487dd-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="487dd-116">String</span></span>|<span data-ttu-id="487dd-p102">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` mit der Komponente „Commands“ gesendet werden </span><span class="sxs-lookup"><span data-stu-id="487dd-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="487dd-119">position</span><span class="sxs-lookup"><span data-stu-id="487dd-119">position</span></span>|<span data-ttu-id="487dd-120">String</span><span class="sxs-lookup"><span data-stu-id="487dd-120">String</span></span>|<span data-ttu-id="487dd-p103">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement. Mögliche Werte sind: `after` (Standardwert) oder `before`.</span><span class="sxs-lookup"><span data-stu-id="487dd-p103">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="487dd-123">target</span><span class="sxs-lookup"><span data-stu-id="487dd-123">target</span></span>|<span data-ttu-id="487dd-124">String</span><span class="sxs-lookup"><span data-stu-id="487dd-124">String</span></span>|<span data-ttu-id="487dd-p104">Das zu aktualisierende Element. Muss die `#<data-id>` oder die generierte `<id>` des Elements oder das Schlüsselwort `body` oder `title` sein.</span><span class="sxs-lookup"><span data-stu-id="487dd-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patchcontentcommand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
