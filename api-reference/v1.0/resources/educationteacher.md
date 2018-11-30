---
title: educationTeacher-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.
ms.openlocfilehash: 59d3334b7a01b0dd39c357f6598085cd78d1e3ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016869"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="60445-103">educationTeacher-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60445-103">educationTeacher resource type</span></span>

<span data-ttu-id="60445-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.</span><span class="sxs-lookup"><span data-stu-id="60445-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="60445-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60445-105">Properties</span></span>
| <span data-ttu-id="60445-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60445-106">Property</span></span>     | <span data-ttu-id="60445-107">Typ</span><span class="sxs-lookup"><span data-stu-id="60445-107">Type</span></span>   |<span data-ttu-id="60445-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60445-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60445-109">externalId</span><span class="sxs-lookup"><span data-stu-id="60445-109">externalId</span></span>|<span data-ttu-id="60445-110">String</span><span class="sxs-lookup"><span data-stu-id="60445-110">String</span></span>| <span data-ttu-id="60445-111">Die ID der Lehrkraft im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="60445-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="60445-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="60445-112">teacherNumber</span></span>|<span data-ttu-id="60445-113">String</span><span class="sxs-lookup"><span data-stu-id="60445-113">String</span></span>|<span data-ttu-id="60445-114">Lehrernummer</span><span class="sxs-lookup"><span data-stu-id="60445-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60445-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60445-115">JSON representation</span></span>

<span data-ttu-id="60445-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60445-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->