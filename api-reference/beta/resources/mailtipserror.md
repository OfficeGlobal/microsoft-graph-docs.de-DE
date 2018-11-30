---
title: Ressourcentyp mailTipsError
description: Ein Fehler, der während einer Aktion auftritt.
ms.openlocfilehash: 94ab795d5cb12c2ff8490806326968d363e1a761
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064685"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="bf821-103">Ressourcentyp mailTipsError</span><span class="sxs-lookup"><span data-stu-id="bf821-103">mailTipsError resource type</span></span>

> <span data-ttu-id="bf821-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bf821-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf821-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf821-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf821-106">Ein Fehler, der während einer Aktion auftritt.</span><span class="sxs-lookup"><span data-stu-id="bf821-106">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="bf821-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bf821-107">Properties</span></span>
| <span data-ttu-id="bf821-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf821-108">Property</span></span>     | <span data-ttu-id="bf821-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bf821-109">Type</span></span>   |<span data-ttu-id="bf821-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf821-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="bf821-111">message</span><span class="sxs-lookup"><span data-stu-id="bf821-111">message</span></span> | <span data-ttu-id="bf821-112">String</span><span class="sxs-lookup"><span data-stu-id="bf821-112">String</span></span> | <span data-ttu-id="bf821-113">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="bf821-113">The error message.</span></span> |
| <span data-ttu-id="bf821-114">code</span><span class="sxs-lookup"><span data-stu-id="bf821-114">code</span></span> | <span data-ttu-id="bf821-115">String</span><span class="sxs-lookup"><span data-stu-id="bf821-115">String</span></span> | <span data-ttu-id="bf821-116">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="bf821-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bf821-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bf821-117">JSON representation</span></span>

<span data-ttu-id="bf821-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bf821-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->