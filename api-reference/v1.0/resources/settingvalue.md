---
title: settingValue-Ressourcentyp
description: Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020091"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="01a4d-103">settingValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="01a4d-103">settingValue resource type</span></span>

<span data-ttu-id="01a4d-104">Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="01a4d-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="01a4d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01a4d-105">Properties</span></span>

| <span data-ttu-id="01a4d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01a4d-106">Property</span></span> | <span data-ttu-id="01a4d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="01a4d-107">Type</span></span> | <span data-ttu-id="01a4d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01a4d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="01a4d-109">name</span><span class="sxs-lookup"><span data-stu-id="01a4d-109">name</span></span>|<span data-ttu-id="01a4d-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01a4d-110">String</span></span>| <span data-ttu-id="01a4d-111">Name der Einstellung (entsprechend der [groupSettingTemplate](groupsettingtemplate.md)-Definition).</span><span class="sxs-lookup"><span data-stu-id="01a4d-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="01a4d-112">Wert</span><span class="sxs-lookup"><span data-stu-id="01a4d-112">value</span></span>|<span data-ttu-id="01a4d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01a4d-113">String</span></span>| <span data-ttu-id="01a4d-114">Wert der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="01a4d-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="01a4d-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01a4d-115">JSON representation</span></span>

<span data-ttu-id="01a4d-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="01a4d-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->