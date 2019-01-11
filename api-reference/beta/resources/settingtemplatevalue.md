---
title: settingTemplateValue-Ressourcentyp
description: Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.
localization_priority: Normal
ms.openlocfilehash: e941630ab72363db1c4be40079cf2af9e40ff002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811865"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="6678e-103">settingTemplateValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6678e-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="6678e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6678e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6678e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6678e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6678e-106">Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.</span><span class="sxs-lookup"><span data-stu-id="6678e-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="6678e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6678e-107">Properties</span></span>
| <span data-ttu-id="6678e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6678e-108">Property</span></span>     | <span data-ttu-id="6678e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6678e-109">Type</span></span>   |<span data-ttu-id="6678e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6678e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6678e-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="6678e-111">defaultValue</span></span>|<span data-ttu-id="6678e-112">string</span><span class="sxs-lookup"><span data-stu-id="6678e-112">string</span></span>|<span data-ttu-id="6678e-113">Der Standardwert für die Einstellung.</span><span class="sxs-lookup"><span data-stu-id="6678e-113">Default value for the setting.</span></span> <span data-ttu-id="6678e-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6678e-114">Read-only.</span></span>|
|<span data-ttu-id="6678e-115">description</span><span class="sxs-lookup"><span data-stu-id="6678e-115">description</span></span>|<span data-ttu-id="6678e-116">string</span><span class="sxs-lookup"><span data-stu-id="6678e-116">string</span></span>|<span data-ttu-id="6678e-117">Beschreibung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="6678e-117">Description of the setting.</span></span> <span data-ttu-id="6678e-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6678e-118">Read-only.</span></span>|
|<span data-ttu-id="6678e-119">name</span><span class="sxs-lookup"><span data-stu-id="6678e-119">name</span></span>|<span data-ttu-id="6678e-120">string</span><span class="sxs-lookup"><span data-stu-id="6678e-120">string</span></span>|<span data-ttu-id="6678e-121">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="6678e-121">Name of the setting.</span></span> <span data-ttu-id="6678e-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6678e-122">Read-only.</span></span>|
|<span data-ttu-id="6678e-123">type</span><span class="sxs-lookup"><span data-stu-id="6678e-123">type</span></span>|<span data-ttu-id="6678e-124">string</span><span class="sxs-lookup"><span data-stu-id="6678e-124">string</span></span>|<span data-ttu-id="6678e-125">Der Typ der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="6678e-125">Type of the setting.</span></span> <span data-ttu-id="6678e-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6678e-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6678e-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6678e-127">JSON representation</span></span>

<span data-ttu-id="6678e-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6678e-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
