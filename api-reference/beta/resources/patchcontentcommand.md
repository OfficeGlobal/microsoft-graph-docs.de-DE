---
title: patchContentCommand-Ressourcentyp
description: Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.
ms.openlocfilehash: fb559a96aa5eef94dd07280b888da0df989b2363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064939"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="a4082-103">patchContentCommand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a4082-103">patchContentCommand resource type</span></span>

> <span data-ttu-id="a4082-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a4082-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4082-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4082-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4082-106">Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4082-106">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4082-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a4082-107">JSON representation</span></span>

<span data-ttu-id="a4082-108">Es folgt eine JSON-Darstellung der Ressource, die im Text der Anforderung [PATCH pages/{id}\`](../api/page-update.md) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="a4082-108">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="a4082-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a4082-109">Properties</span></span>
| <span data-ttu-id="a4082-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4082-110">Property</span></span>     | <span data-ttu-id="a4082-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a4082-111">Type</span></span>   |<span data-ttu-id="a4082-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4082-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4082-113">action</span><span class="sxs-lookup"><span data-stu-id="a4082-113">action</span></span>|<span data-ttu-id="a4082-114">String</span><span class="sxs-lookup"><span data-stu-id="a4082-114">String</span></span>|<span data-ttu-id="a4082-p102">Die für das Zielelement auszuführende Aktion. Mögliche Werte sind: `replace`, `append`, `delete`, `insert` oder `prepend`.</span><span class="sxs-lookup"><span data-stu-id="a4082-p102">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="a4082-117">content</span><span class="sxs-lookup"><span data-stu-id="a4082-117">content</span></span>|<span data-ttu-id="a4082-118">String</span><span class="sxs-lookup"><span data-stu-id="a4082-118">String</span></span>|<span data-ttu-id="a4082-p103">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` mit der Komponente „Commands“ gesendet werden </span><span class="sxs-lookup"><span data-stu-id="a4082-p103">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="a4082-121">position</span><span class="sxs-lookup"><span data-stu-id="a4082-121">position</span></span>|<span data-ttu-id="a4082-122">String</span><span class="sxs-lookup"><span data-stu-id="a4082-122">String</span></span>|<span data-ttu-id="a4082-p104">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement. Mögliche Werte sind: `after` (Standardwert) oder `before`.</span><span class="sxs-lookup"><span data-stu-id="a4082-p104">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="a4082-125">target</span><span class="sxs-lookup"><span data-stu-id="a4082-125">target</span></span>|<span data-ttu-id="a4082-126">String</span><span class="sxs-lookup"><span data-stu-id="a4082-126">String</span></span>|<span data-ttu-id="a4082-p105">Das zu aktualisierende Element. Muss die `#<data-id>` oder die generierte `<id>` des Elements oder das Schlüsselwort `body` oder `title` sein.</span><span class="sxs-lookup"><span data-stu-id="a4082-p105">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->