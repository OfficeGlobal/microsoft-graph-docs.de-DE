---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: c65b3cf021321a7e021c5fa4193abdcdce6c635a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520606"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="f12e3-102">VersionAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f12e3-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f12e3-103">Wenn die **VersionAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität eine neue Version erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="f12e3-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f12e3-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f12e3-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f12e3-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f12e3-105">Properties</span></span>

| <span data-ttu-id="f12e3-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f12e3-106">Property name</span></span> | <span data-ttu-id="f12e3-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f12e3-107">Type</span></span>   | <span data-ttu-id="f12e3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f12e3-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f12e3-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="f12e3-109">newVersion</span></span>    | <span data-ttu-id="f12e3-110">string</span><span class="sxs-lookup"><span data-stu-id="f12e3-110">string</span></span> | <span data-ttu-id="f12e3-111">Der Name der neuen Version, die von dieser Aktion erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f12e3-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="f12e3-112">Hinweise</span><span class="sxs-lookup"><span data-stu-id="f12e3-112">Remarks</span></span>

<span data-ttu-id="f12e3-113">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f12e3-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/versionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
