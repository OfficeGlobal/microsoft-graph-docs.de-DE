---
title: educationTeacher-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b58d74e6b53b1721a5139d050c7e89197b8721be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929557"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="43fc8-103">educationTeacher-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="43fc8-103">educationTeacher resource type</span></span>

<span data-ttu-id="43fc8-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.</span><span class="sxs-lookup"><span data-stu-id="43fc8-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="43fc8-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="43fc8-105">Properties</span></span>
| <span data-ttu-id="43fc8-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43fc8-106">Property</span></span>     | <span data-ttu-id="43fc8-107">Typ</span><span class="sxs-lookup"><span data-stu-id="43fc8-107">Type</span></span>   |<span data-ttu-id="43fc8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43fc8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43fc8-109">externalId</span><span class="sxs-lookup"><span data-stu-id="43fc8-109">externalId</span></span>|<span data-ttu-id="43fc8-110">String</span><span class="sxs-lookup"><span data-stu-id="43fc8-110">String</span></span>| <span data-ttu-id="43fc8-111">Die ID der Lehrkraft im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="43fc8-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="43fc8-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="43fc8-112">teacherNumber</span></span>|<span data-ttu-id="43fc8-113">String</span><span class="sxs-lookup"><span data-stu-id="43fc8-113">String</span></span>|<span data-ttu-id="43fc8-114">Lehrernummer</span><span class="sxs-lookup"><span data-stu-id="43fc8-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43fc8-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43fc8-115">JSON representation</span></span>

<span data-ttu-id="43fc8-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43fc8-116">The following is a JSON representation of the resource.</span></span>

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
