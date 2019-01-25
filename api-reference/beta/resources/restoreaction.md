---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: f04f9811cefba60d0b06b99605774fb8fbfa0125
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514075"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="c9231-102">RestoreAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9231-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9231-103">Wenn die **RestoreAction**-Ressource für ein [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element erneut gespeichert hat.</span><span class="sxs-lookup"><span data-stu-id="c9231-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="c9231-104">**Hinweis**: Diese Ressource ist heute zwar leer, in künftigen API-Überarbeitungen wird die Ressource aber möglicherweise mit weiteren Eigenschaften gefüllt.</span><span class="sxs-lookup"><span data-stu-id="c9231-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c9231-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9231-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="c9231-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9231-106">Properties</span></span>

<span data-ttu-id="c9231-107">Keine.</span><span class="sxs-lookup"><span data-stu-id="c9231-107">None.</span></span> <span data-ttu-id="c9231-108">Dieses Facet ist ein NULL- oder Nicht-NULL-Wert und enthält keine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c9231-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="c9231-109">Hinweise</span><span class="sxs-lookup"><span data-stu-id="c9231-109">Remarks</span></span>

<span data-ttu-id="c9231-110">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c9231-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/restoreaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
