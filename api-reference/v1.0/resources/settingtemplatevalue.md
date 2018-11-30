---
title: settingTemplateValue-Ressourcentyp
description: Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.
ms.openlocfilehash: 00e424e36338855d8ef603d06c7a9ee52a99c621
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019498"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="f367c-103">settingTemplateValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f367c-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="f367c-104">Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.</span><span class="sxs-lookup"><span data-stu-id="f367c-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="f367c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f367c-105">Properties</span></span>

| <span data-ttu-id="f367c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f367c-106">Property</span></span> | <span data-ttu-id="f367c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f367c-107">Type</span></span> | <span data-ttu-id="f367c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f367c-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f367c-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="f367c-109">defaultValue</span></span>|<span data-ttu-id="f367c-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f367c-110">String</span></span>| <span data-ttu-id="f367c-111">Der Standardwert für die Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f367c-111">Default value for the setting.</span></span> |
|<span data-ttu-id="f367c-112">description</span><span class="sxs-lookup"><span data-stu-id="f367c-112">description</span></span>|<span data-ttu-id="f367c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f367c-113">String</span></span>| <span data-ttu-id="f367c-114">Beschreibung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f367c-114">Description of the setting.</span></span> |
|<span data-ttu-id="f367c-115">Name</span><span class="sxs-lookup"><span data-stu-id="f367c-115">name</span></span>|<span data-ttu-id="f367c-116">String</span><span class="sxs-lookup"><span data-stu-id="f367c-116">String</span></span>| <span data-ttu-id="f367c-117">Der Name der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f367c-117">Name of the setting.</span></span> |
|<span data-ttu-id="f367c-118">type</span><span class="sxs-lookup"><span data-stu-id="f367c-118">type</span></span>|<span data-ttu-id="f367c-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f367c-119">String</span></span>| <span data-ttu-id="f367c-120">Der Typ der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f367c-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="f367c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f367c-121">JSON representation</span></span>

<span data-ttu-id="f367c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f367c-122">Here is a JSON representation of the resource.</span></span>

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