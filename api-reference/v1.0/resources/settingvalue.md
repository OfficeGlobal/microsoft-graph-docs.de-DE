---
title: settingValue-Ressourcentyp
description: Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834034"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="19990-103">settingValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="19990-103">settingValue resource type</span></span>

<span data-ttu-id="19990-104">Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="19990-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="19990-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19990-105">Properties</span></span>

| <span data-ttu-id="19990-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19990-106">Property</span></span> | <span data-ttu-id="19990-107">Typ</span><span class="sxs-lookup"><span data-stu-id="19990-107">Type</span></span> | <span data-ttu-id="19990-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19990-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="19990-109">name</span><span class="sxs-lookup"><span data-stu-id="19990-109">name</span></span>|<span data-ttu-id="19990-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19990-110">String</span></span>| <span data-ttu-id="19990-111">Name der Einstellung (entsprechend der [groupSettingTemplate](groupsettingtemplate.md)-Definition).</span><span class="sxs-lookup"><span data-stu-id="19990-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="19990-112">Wert</span><span class="sxs-lookup"><span data-stu-id="19990-112">value</span></span>|<span data-ttu-id="19990-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19990-113">String</span></span>| <span data-ttu-id="19990-114">Wert der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="19990-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="19990-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19990-115">JSON representation</span></span>

<span data-ttu-id="19990-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19990-116">Here is a JSON representation of the resource.</span></span>

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
