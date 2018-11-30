---
title: settingTemplateValue-Ressourcentyp
description: Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.
ms.openlocfilehash: afc872f3e3d8d02acae639b967cdaf9375bb60cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061471"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="91025-103">settingTemplateValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91025-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="91025-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91025-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91025-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91025-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91025-106">Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.</span><span class="sxs-lookup"><span data-stu-id="91025-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="91025-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91025-107">Properties</span></span>
| <span data-ttu-id="91025-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91025-108">Property</span></span>     | <span data-ttu-id="91025-109">Typ</span><span class="sxs-lookup"><span data-stu-id="91025-109">Type</span></span>   |<span data-ttu-id="91025-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91025-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91025-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="91025-111">defaultValue</span></span>|<span data-ttu-id="91025-112">string</span><span class="sxs-lookup"><span data-stu-id="91025-112">string</span></span>|<span data-ttu-id="91025-113">Der Standardwert für die Einstellung.</span><span class="sxs-lookup"><span data-stu-id="91025-113">Default value for the setting.</span></span> <span data-ttu-id="91025-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91025-114">Read-only.</span></span>|
|<span data-ttu-id="91025-115">description</span><span class="sxs-lookup"><span data-stu-id="91025-115">description</span></span>|<span data-ttu-id="91025-116">string</span><span class="sxs-lookup"><span data-stu-id="91025-116">string</span></span>|<span data-ttu-id="91025-117">Beschreibung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="91025-117">Description of the setting.</span></span> <span data-ttu-id="91025-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91025-118">Read-only.</span></span>|
|<span data-ttu-id="91025-119">name</span><span class="sxs-lookup"><span data-stu-id="91025-119">name</span></span>|<span data-ttu-id="91025-120">string</span><span class="sxs-lookup"><span data-stu-id="91025-120">string</span></span>|<span data-ttu-id="91025-121">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="91025-121">Name of the setting.</span></span> <span data-ttu-id="91025-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91025-122">Read-only.</span></span>|
|<span data-ttu-id="91025-123">Typ</span><span class="sxs-lookup"><span data-stu-id="91025-123">type</span></span>|<span data-ttu-id="91025-124">string</span><span class="sxs-lookup"><span data-stu-id="91025-124">string</span></span>|<span data-ttu-id="91025-125">Der Typ der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="91025-125">Type of the setting.</span></span> <span data-ttu-id="91025-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91025-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91025-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91025-127">JSON representation</span></span>

<span data-ttu-id="91025-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91025-128">Here is a JSON representation of the resource.</span></span>

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
