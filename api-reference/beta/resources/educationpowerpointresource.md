---
title: Ressourcentyp educationPowerPointResource
description: 'Eine Unterklasse der EducationResource. Hierbei handelt es sich um eine PowerPoint-Ressource. PowerPoint-Datei muss im Zusammenhang mit **FileResource** Verzeichnis hochgeladen werden die '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512199"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="8989b-105">Ressourcentyp educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="8989b-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8989b-106">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="8989b-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="8989b-107">Hierbei handelt es sich um eine PowerPoint-Ressource.</span><span class="sxs-lookup"><span data-stu-id="8989b-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="8989b-108">PowerPoint-Datei muss im Verzeichnis **FileResource** zugeordnet, die Zuordnung oder die Übermittlung hochgeladen werden.</span><span class="sxs-lookup"><span data-stu-id="8989b-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="8989b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8989b-109">Properties</span></span>
| <span data-ttu-id="8989b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8989b-110">Property</span></span>     | <span data-ttu-id="8989b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8989b-111">Type</span></span>   |<span data-ttu-id="8989b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8989b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8989b-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="8989b-113">fileUrl</span></span>|<span data-ttu-id="8989b-114">String</span><span class="sxs-lookup"><span data-stu-id="8989b-114">String</span></span>|<span data-ttu-id="8989b-115">Speicherort der Datei auf dem Datenträger.</span><span class="sxs-lookup"><span data-stu-id="8989b-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8989b-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8989b-116">JSON representation</span></span>

<span data-ttu-id="8989b-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8989b-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
