---
title: settingValue-Ressourcentyp
description: Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.
ms.openlocfilehash: fb1c249fba9506b2a4c6ad29d04f98b36c82f53f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063530"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="1e391-103">settingValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1e391-103">settingValue resource type</span></span>

> <span data-ttu-id="1e391-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e391-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e391-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e391-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e391-106">Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="1e391-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="1e391-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1e391-107">Properties</span></span>
| <span data-ttu-id="1e391-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e391-108">Property</span></span>     | <span data-ttu-id="1e391-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1e391-109">Type</span></span>   |<span data-ttu-id="1e391-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e391-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e391-111">name</span><span class="sxs-lookup"><span data-stu-id="1e391-111">name</span></span>|<span data-ttu-id="1e391-112">string</span><span class="sxs-lookup"><span data-stu-id="1e391-112">string</span></span>|<span data-ttu-id="1e391-113">Name der Einstellung (wie die DirectorySettingTemplate definiert).</span><span class="sxs-lookup"><span data-stu-id="1e391-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="1e391-114">Wert</span><span class="sxs-lookup"><span data-stu-id="1e391-114">value</span></span>|<span data-ttu-id="1e391-115">string</span><span class="sxs-lookup"><span data-stu-id="1e391-115">string</span></span>|<span data-ttu-id="1e391-116">Wert der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="1e391-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e391-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1e391-117">JSON representation</span></span>

<span data-ttu-id="1e391-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e391-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
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
