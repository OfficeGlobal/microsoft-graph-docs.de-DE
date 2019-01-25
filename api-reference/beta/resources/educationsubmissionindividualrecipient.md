---
title: Ressourcentyp educationSubmissionIndividualRecipient
description: 'Eine Unterklasse der EducationSubmissionRecipient, der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8660ec569362d8170d15de86073c0ef59c9ec0a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519185"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="e7579-103">Ressourcentyp educationSubmissionIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="e7579-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7579-104">Eine Unterklasse der [EducationSubmissionRecipient](educationsubmissionrecipient.md) , der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="e7579-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="e7579-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e7579-105">Properties</span></span>
| <span data-ttu-id="e7579-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7579-106">Property</span></span>     | <span data-ttu-id="e7579-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e7579-107">Type</span></span>   |<span data-ttu-id="e7579-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7579-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7579-109">userId</span><span class="sxs-lookup"><span data-stu-id="e7579-109">userId</span></span>|<span data-ttu-id="e7579-110">String</span><span class="sxs-lookup"><span data-stu-id="e7579-110">String</span></span>|<span data-ttu-id="e7579-111">Benutzer-ID des Benutzers, dem die Übermittlung zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="e7579-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7579-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e7579-112">JSON representation</span></span>

<span data-ttu-id="e7579-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e7579-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
