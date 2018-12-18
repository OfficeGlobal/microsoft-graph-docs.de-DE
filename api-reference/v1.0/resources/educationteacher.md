---
title: educationTeacher-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.
author: mmast-msft
ms.openlocfilehash: a880c3908b70e0b9d7c580492f45183b8f15425d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334461"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="536e9-103">educationTeacher-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="536e9-103">educationTeacher resource type</span></span>

<span data-ttu-id="536e9-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.</span><span class="sxs-lookup"><span data-stu-id="536e9-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="536e9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="536e9-105">Properties</span></span>
| <span data-ttu-id="536e9-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="536e9-106">Property</span></span>     | <span data-ttu-id="536e9-107">Typ</span><span class="sxs-lookup"><span data-stu-id="536e9-107">Type</span></span>   |<span data-ttu-id="536e9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="536e9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="536e9-109">externalId</span><span class="sxs-lookup"><span data-stu-id="536e9-109">externalId</span></span>|<span data-ttu-id="536e9-110">String</span><span class="sxs-lookup"><span data-stu-id="536e9-110">String</span></span>| <span data-ttu-id="536e9-111">Die ID der Lehrkraft im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="536e9-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="536e9-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="536e9-112">teacherNumber</span></span>|<span data-ttu-id="536e9-113">String</span><span class="sxs-lookup"><span data-stu-id="536e9-113">String</span></span>|<span data-ttu-id="536e9-114">Lehrernummer</span><span class="sxs-lookup"><span data-stu-id="536e9-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="536e9-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="536e9-115">JSON representation</span></span>

<span data-ttu-id="536e9-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="536e9-116">The following is a JSON representation of the resource.</span></span>

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