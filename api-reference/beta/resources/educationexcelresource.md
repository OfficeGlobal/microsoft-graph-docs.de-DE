---
title: Ressourcentyp educationExcelResource
description: 'Eine Unterklasse der EducationResource. Dieser Ressourcentyp stellt ein Excel-Dokument dar.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522420"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="e6370-104">Ressourcentyp educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="e6370-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6370-105">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="e6370-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="e6370-106">Dieser Ressourcentyp stellt ein Excel-Dokument dar.</span><span class="sxs-lookup"><span data-stu-id="e6370-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="e6370-107">**Hinweis:** Die Excel-Datei muss im Ordner "Resource" die Zuordnung oder Übermittlung-Objekt zu dem diese Ressource gehört zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="e6370-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="e6370-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6370-108">Properties</span></span>
| <span data-ttu-id="e6370-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6370-109">Property</span></span>     | <span data-ttu-id="e6370-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e6370-110">Type</span></span>   |<span data-ttu-id="e6370-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6370-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6370-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="e6370-112">fileUrl</span></span>|<span data-ttu-id="e6370-113">String</span><span class="sxs-lookup"><span data-stu-id="e6370-113">String</span></span>|<span data-ttu-id="e6370-114">Zeiger auf das Excel-File-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e6370-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6370-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6370-115">JSON representation</span></span>

<span data-ttu-id="e6370-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6370-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationexcelresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
