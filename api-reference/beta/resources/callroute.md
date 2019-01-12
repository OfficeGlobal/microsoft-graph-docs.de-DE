---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd131afcdb5581a719107d9fd3a9a597979d6f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933071"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="f193e-103">Ressourcentyp callRoute</span><span class="sxs-lookup"><span data-stu-id="f193e-103">callRoute resource type</span></span>

> <span data-ttu-id="f193e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f193e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f193e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f193e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f193e-106">Der Typ des CallRoute.</span><span class="sxs-lookup"><span data-stu-id="f193e-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="f193e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f193e-107">Properties</span></span>

| <span data-ttu-id="f193e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f193e-108">Property</span></span>            | <span data-ttu-id="f193e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f193e-109">Type</span></span>                          | <span data-ttu-id="f193e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f193e-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f193e-111">endgültige</span><span class="sxs-lookup"><span data-stu-id="f193e-111">final</span></span>               | [<span data-ttu-id="f193e-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="f193e-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="f193e-113">Die Identität, die in die Unterhaltung aufgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="f193e-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="f193e-114">Original</span><span class="sxs-lookup"><span data-stu-id="f193e-114">original</span></span>            | [<span data-ttu-id="f193e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="f193e-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="f193e-116">Die Identität, die ursprünglich in den Anruf verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="f193e-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="f193e-117">routingType</span><span class="sxs-lookup"><span data-stu-id="f193e-117">routingType</span></span>         | <span data-ttu-id="f193e-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f193e-118">String</span></span>                        | <span data-ttu-id="f193e-119">Mögliche Werte sind: `forwarded`, `lookup` und `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="f193e-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f193e-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f193e-120">JSON representation</span></span>

<span data-ttu-id="f193e-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f193e-121">The following is a JSON representation of the resource.</span></span>

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
