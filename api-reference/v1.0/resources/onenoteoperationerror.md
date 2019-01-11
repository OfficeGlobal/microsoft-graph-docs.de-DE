---
title: onenoteOperationError-Ressourcentyp
description: Ein Fehler einem OneNote-Vorgang, der nicht ausgeführt werden konnte.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: df0bfd768d26c751a303f42e1f1123b863388faa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837338"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="21216-103">onenoteOperationError-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="21216-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="21216-104">Ein Fehler einem OneNote-Vorgang, der nicht ausgeführt werden konnte.</span><span class="sxs-lookup"><span data-stu-id="21216-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21216-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21216-105">JSON representation</span></span>

<span data-ttu-id="21216-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21216-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="21216-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21216-107">Properties</span></span>
| <span data-ttu-id="21216-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21216-108">Property</span></span>     | <span data-ttu-id="21216-109">Typ</span><span class="sxs-lookup"><span data-stu-id="21216-109">Type</span></span>   |<span data-ttu-id="21216-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21216-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21216-111">code</span><span class="sxs-lookup"><span data-stu-id="21216-111">code</span></span>|<span data-ttu-id="21216-112">string</span><span class="sxs-lookup"><span data-stu-id="21216-112">string</span></span>|<span data-ttu-id="21216-113">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="21216-113">The error code.</span></span>|
|<span data-ttu-id="21216-114">message</span><span class="sxs-lookup"><span data-stu-id="21216-114">message</span></span>|<span data-ttu-id="21216-115">string</span><span class="sxs-lookup"><span data-stu-id="21216-115">string</span></span>|<span data-ttu-id="21216-116">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="21216-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
