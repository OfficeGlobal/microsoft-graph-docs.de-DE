---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: 5e3b7cbf752d3ddb2c4b7bde3981d2a443028b92
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512619"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="ab420-102">DeleteAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ab420-102">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab420-103">Wenn eine **DeleteAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element gelöscht hat.</span><span class="sxs-lookup"><span data-stu-id="ab420-103">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="ab420-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab420-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a><span data-ttu-id="ab420-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab420-105">Properties</span></span>

| <span data-ttu-id="ab420-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ab420-106">Property name</span></span> | <span data-ttu-id="ab420-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ab420-107">Type</span></span>   | <span data-ttu-id="ab420-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab420-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ab420-109">name</span><span class="sxs-lookup"><span data-stu-id="ab420-109">name</span></span>          | <span data-ttu-id="ab420-110">string</span><span class="sxs-lookup"><span data-stu-id="ab420-110">string</span></span> | <span data-ttu-id="ab420-111">Der Name des Elements, das gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="ab420-111">The name of the item that was deleted.</span></span>
| <span data-ttu-id="ab420-112">objectType</span><span class="sxs-lookup"><span data-stu-id="ab420-112">objectType</span></span>    | <span data-ttu-id="ab420-113">string</span><span class="sxs-lookup"><span data-stu-id="ab420-113">string</span></span> | <span data-ttu-id="ab420-114">`File`oder `Folder`, je nach Typ des gelöschten Elements.</span><span class="sxs-lookup"><span data-stu-id="ab420-114">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="ab420-115">Hinweise</span><span class="sxs-lookup"><span data-stu-id="ab420-115">Remarks</span></span>

<span data-ttu-id="ab420-116">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ab420-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleteaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
