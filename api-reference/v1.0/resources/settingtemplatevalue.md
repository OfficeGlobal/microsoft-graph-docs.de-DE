---
title: settingTemplateValue-Ressourcentyp
description: Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828322"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="88a37-103">settingTemplateValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88a37-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="88a37-104">Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.</span><span class="sxs-lookup"><span data-stu-id="88a37-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="88a37-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88a37-105">Properties</span></span>

| <span data-ttu-id="88a37-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88a37-106">Property</span></span> | <span data-ttu-id="88a37-107">Typ</span><span class="sxs-lookup"><span data-stu-id="88a37-107">Type</span></span> | <span data-ttu-id="88a37-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88a37-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="88a37-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="88a37-109">defaultValue</span></span>|<span data-ttu-id="88a37-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88a37-110">String</span></span>| <span data-ttu-id="88a37-111">Der Standardwert für die Einstellung.</span><span class="sxs-lookup"><span data-stu-id="88a37-111">Default value for the setting.</span></span> |
|<span data-ttu-id="88a37-112">description</span><span class="sxs-lookup"><span data-stu-id="88a37-112">description</span></span>|<span data-ttu-id="88a37-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88a37-113">String</span></span>| <span data-ttu-id="88a37-114">Beschreibung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="88a37-114">Description of the setting.</span></span> |
|<span data-ttu-id="88a37-115">Name</span><span class="sxs-lookup"><span data-stu-id="88a37-115">name</span></span>|<span data-ttu-id="88a37-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88a37-116">String</span></span>| <span data-ttu-id="88a37-117">Der Name der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="88a37-117">Name of the setting.</span></span> |
|<span data-ttu-id="88a37-118">type</span><span class="sxs-lookup"><span data-stu-id="88a37-118">type</span></span>|<span data-ttu-id="88a37-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88a37-119">String</span></span>| <span data-ttu-id="88a37-120">Der Typ der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="88a37-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="88a37-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88a37-121">JSON representation</span></span>

<span data-ttu-id="88a37-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88a37-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
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
