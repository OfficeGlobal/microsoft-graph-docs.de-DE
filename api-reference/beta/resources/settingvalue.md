---
title: settingValue-Ressourcentyp
description: Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.
localization_priority: Normal
ms.openlocfilehash: 0ddd6388e14ea3deff99e927541694a97c594195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815526"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="aad1f-103">settingValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aad1f-103">settingValue resource type</span></span>

> <span data-ttu-id="aad1f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aad1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aad1f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aad1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aad1f-106">Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="aad1f-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="aad1f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aad1f-107">Properties</span></span>
| <span data-ttu-id="aad1f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aad1f-108">Property</span></span>     | <span data-ttu-id="aad1f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="aad1f-109">Type</span></span>   |<span data-ttu-id="aad1f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aad1f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aad1f-111">name</span><span class="sxs-lookup"><span data-stu-id="aad1f-111">name</span></span>|<span data-ttu-id="aad1f-112">string</span><span class="sxs-lookup"><span data-stu-id="aad1f-112">string</span></span>|<span data-ttu-id="aad1f-113">Name der Einstellung (wie die DirectorySettingTemplate definiert).</span><span class="sxs-lookup"><span data-stu-id="aad1f-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="aad1f-114">Wert</span><span class="sxs-lookup"><span data-stu-id="aad1f-114">value</span></span>|<span data-ttu-id="aad1f-115">string</span><span class="sxs-lookup"><span data-stu-id="aad1f-115">string</span></span>|<span data-ttu-id="aad1f-116">Wert der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="aad1f-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aad1f-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aad1f-117">JSON representation</span></span>

<span data-ttu-id="aad1f-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aad1f-118">Here is a JSON representation of the resource.</span></span>

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
