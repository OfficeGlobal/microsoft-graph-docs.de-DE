---
title: onenoteOperationError-Ressourcentyp
description: Ein Fehler einem OneNote-Vorgang, der nicht ausgeführt werden konnte.
author: Jewan-microsoft
ms.openlocfilehash: 4cba6de22f08e2e41f281863e3494fbb589e6e41
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354782"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="27d10-103">onenoteOperationError-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27d10-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="27d10-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="27d10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27d10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27d10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27d10-106">Ein Fehler einem OneNote-Vorgang, der nicht ausgeführt werden konnte.</span><span class="sxs-lookup"><span data-stu-id="27d10-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27d10-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27d10-107">JSON representation</span></span>

<span data-ttu-id="27d10-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27d10-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="27d10-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27d10-109">Properties</span></span>
| <span data-ttu-id="27d10-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27d10-110">Property</span></span>     | <span data-ttu-id="27d10-111">Typ</span><span class="sxs-lookup"><span data-stu-id="27d10-111">Type</span></span>   |<span data-ttu-id="27d10-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27d10-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27d10-113">code</span><span class="sxs-lookup"><span data-stu-id="27d10-113">code</span></span>|<span data-ttu-id="27d10-114">string</span><span class="sxs-lookup"><span data-stu-id="27d10-114">string</span></span>|<span data-ttu-id="27d10-115">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="27d10-115">The error code.</span></span>|
|<span data-ttu-id="27d10-116">message</span><span class="sxs-lookup"><span data-stu-id="27d10-116">message</span></span>|<span data-ttu-id="27d10-117">string</span><span class="sxs-lookup"><span data-stu-id="27d10-117">string</span></span>|<span data-ttu-id="27d10-118">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="27d10-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
