---
title: educationTeacher-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen `teacher` hinzugefügt werden, wenn die primaryRole eines Benutzers  ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 17019d5ff5c2bc9614e934ef66d63e459371469a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510855"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="82b6e-103">educationTeacher-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="82b6e-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82b6e-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.</span><span class="sxs-lookup"><span data-stu-id="82b6e-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="82b6e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="82b6e-105">Properties</span></span>
| <span data-ttu-id="82b6e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82b6e-106">Property</span></span>     | <span data-ttu-id="82b6e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="82b6e-107">Type</span></span>   |<span data-ttu-id="82b6e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82b6e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82b6e-109">externalId</span><span class="sxs-lookup"><span data-stu-id="82b6e-109">externalId</span></span>|<span data-ttu-id="82b6e-110">String</span><span class="sxs-lookup"><span data-stu-id="82b6e-110">String</span></span>| <span data-ttu-id="82b6e-111">Die ID der Lehrkraft im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="82b6e-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="82b6e-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="82b6e-112">teacherNumber</span></span>|<span data-ttu-id="82b6e-113">String</span><span class="sxs-lookup"><span data-stu-id="82b6e-113">String</span></span>|<span data-ttu-id="82b6e-114">Lehrernummer</span><span class="sxs-lookup"><span data-stu-id="82b6e-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82b6e-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="82b6e-115">JSON representation</span></span>

<span data-ttu-id="82b6e-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="82b6e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationteacher.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
