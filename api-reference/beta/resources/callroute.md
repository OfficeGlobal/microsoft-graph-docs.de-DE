---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
ms.openlocfilehash: d2a85d34fe755c6e725abc9a1308a3837f0acf3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060373"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="1e2e5-103">Ressourcentyp callRoute</span><span class="sxs-lookup"><span data-stu-id="1e2e5-103">callRoute resource type</span></span>

> <span data-ttu-id="1e2e5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e2e5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e2e5-106">Der Typ des CallRoute.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="1e2e5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1e2e5-107">Properties</span></span>

| <span data-ttu-id="1e2e5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e2e5-108">Property</span></span>            | <span data-ttu-id="1e2e5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1e2e5-109">Type</span></span>                          | <span data-ttu-id="1e2e5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e2e5-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1e2e5-111">endgültige</span><span class="sxs-lookup"><span data-stu-id="1e2e5-111">final</span></span>               | [<span data-ttu-id="1e2e5-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="1e2e5-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="1e2e5-113">Die Identität, die in die Unterhaltung aufgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="1e2e5-114">Original</span><span class="sxs-lookup"><span data-stu-id="1e2e5-114">original</span></span>            | [<span data-ttu-id="1e2e5-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="1e2e5-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="1e2e5-116">Die Identität, die ursprünglich in den Anruf verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="1e2e5-117">routingType</span><span class="sxs-lookup"><span data-stu-id="1e2e5-117">routingType</span></span>         | <span data-ttu-id="1e2e5-118">String</span><span class="sxs-lookup"><span data-stu-id="1e2e5-118">String</span></span>                        | <span data-ttu-id="1e2e5-119">Mögliche Werte sind: `forwarded`, `lookup` und `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1e2e5-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1e2e5-120">JSON representation</span></span>

<span data-ttu-id="1e2e5-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e2e5-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
