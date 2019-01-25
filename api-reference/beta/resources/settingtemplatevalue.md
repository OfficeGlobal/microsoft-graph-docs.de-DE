---
title: settingTemplateValue-Ressourcentyp
description: Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528011"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="92698-103">settingTemplateValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="92698-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92698-104">Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.</span><span class="sxs-lookup"><span data-stu-id="92698-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="92698-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92698-105">Properties</span></span>
| <span data-ttu-id="92698-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92698-106">Property</span></span>     | <span data-ttu-id="92698-107">Typ</span><span class="sxs-lookup"><span data-stu-id="92698-107">Type</span></span>   |<span data-ttu-id="92698-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92698-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92698-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="92698-109">defaultValue</span></span>|<span data-ttu-id="92698-110">string</span><span class="sxs-lookup"><span data-stu-id="92698-110">string</span></span>|<span data-ttu-id="92698-111">Der Standardwert für die Einstellung.</span><span class="sxs-lookup"><span data-stu-id="92698-111">Default value for the setting.</span></span> <span data-ttu-id="92698-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92698-112">Read-only.</span></span>|
|<span data-ttu-id="92698-113">description</span><span class="sxs-lookup"><span data-stu-id="92698-113">description</span></span>|<span data-ttu-id="92698-114">string</span><span class="sxs-lookup"><span data-stu-id="92698-114">string</span></span>|<span data-ttu-id="92698-115">Beschreibung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="92698-115">Description of the setting.</span></span> <span data-ttu-id="92698-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92698-116">Read-only.</span></span>|
|<span data-ttu-id="92698-117">name</span><span class="sxs-lookup"><span data-stu-id="92698-117">name</span></span>|<span data-ttu-id="92698-118">string</span><span class="sxs-lookup"><span data-stu-id="92698-118">string</span></span>|<span data-ttu-id="92698-119">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="92698-119">Name of the setting.</span></span> <span data-ttu-id="92698-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92698-120">Read-only.</span></span>|
|<span data-ttu-id="92698-121">type</span><span class="sxs-lookup"><span data-stu-id="92698-121">type</span></span>|<span data-ttu-id="92698-122">string</span><span class="sxs-lookup"><span data-stu-id="92698-122">string</span></span>|<span data-ttu-id="92698-123">Der Typ der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="92698-123">Type of the setting.</span></span> <span data-ttu-id="92698-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="92698-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92698-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92698-125">JSON representation</span></span>

<span data-ttu-id="92698-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92698-126">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/settingtemplatevalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
