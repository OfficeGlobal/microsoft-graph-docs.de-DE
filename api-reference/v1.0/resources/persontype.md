---
title: personType-Ressourcentyp
description: Stellt den Typ der Person dar.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 270fa800242ae7a25ed0f5959a97b6a70f7cedd3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917272"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="2a502-103">personType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2a502-103">personType resource type</span></span>

<span data-ttu-id="2a502-104">Stellt den Typ der Person dar.</span><span class="sxs-lookup"><span data-stu-id="2a502-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2a502-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a502-105">JSON representation</span></span>

<span data-ttu-id="2a502-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a502-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2a502-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a502-107">Properties</span></span>
| <span data-ttu-id="2a502-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a502-108">Property</span></span>     | <span data-ttu-id="2a502-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2a502-109">Type</span></span>   |<span data-ttu-id="2a502-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a502-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a502-111">class</span><span class="sxs-lookup"><span data-stu-id="2a502-111">class</span></span>|<span data-ttu-id="2a502-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a502-112">String</span></span>|<span data-ttu-id="2a502-113">Der Typ der Datenquelle, z. B. Person.</span><span class="sxs-lookup"><span data-stu-id="2a502-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="2a502-114">subclass</span><span class="sxs-lookup"><span data-stu-id="2a502-114">subclass</span></span>|<span data-ttu-id="2a502-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a502-115">String</span></span>|<span data-ttu-id="2a502-116">Der sekundäre Typ der Datenquelle, z. B. OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="2a502-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
