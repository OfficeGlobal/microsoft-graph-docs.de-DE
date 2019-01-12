---
title: onenoteOperationError-Ressourcentyp
description: Ein Fehler einem OneNote-Vorgang, der nicht ausgeführt werden konnte.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 42f9f4777a98081a3fa18c010c301ba19a34b750
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975505"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="38b8c-103">onenoteOperationError-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="38b8c-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="38b8c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="38b8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38b8c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38b8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38b8c-106">Ein Fehler einem OneNote-Vorgang, der nicht ausgeführt werden konnte.</span><span class="sxs-lookup"><span data-stu-id="38b8c-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38b8c-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38b8c-107">JSON representation</span></span>

<span data-ttu-id="38b8c-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38b8c-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="38b8c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38b8c-109">Properties</span></span>
| <span data-ttu-id="38b8c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38b8c-110">Property</span></span>     | <span data-ttu-id="38b8c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="38b8c-111">Type</span></span>   |<span data-ttu-id="38b8c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38b8c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38b8c-113">code</span><span class="sxs-lookup"><span data-stu-id="38b8c-113">code</span></span>|<span data-ttu-id="38b8c-114">string</span><span class="sxs-lookup"><span data-stu-id="38b8c-114">string</span></span>|<span data-ttu-id="38b8c-115">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="38b8c-115">The error code.</span></span>|
|<span data-ttu-id="38b8c-116">message</span><span class="sxs-lookup"><span data-stu-id="38b8c-116">message</span></span>|<span data-ttu-id="38b8c-117">string</span><span class="sxs-lookup"><span data-stu-id="38b8c-117">string</span></span>|<span data-ttu-id="38b8c-118">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="38b8c-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
