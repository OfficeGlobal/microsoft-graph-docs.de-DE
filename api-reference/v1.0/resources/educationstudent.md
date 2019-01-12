---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 683a290806f9a70f97bda4aa9429a64578fbcd97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916362"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="7056e-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7056e-103">educationStudent resource type</span></span>

<span data-ttu-id="7056e-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="7056e-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="7056e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7056e-105">Properties</span></span>
| <span data-ttu-id="7056e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7056e-106">Property</span></span>     | <span data-ttu-id="7056e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7056e-107">Type</span></span>   |<span data-ttu-id="7056e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7056e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7056e-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="7056e-109">birthDate</span></span>|<span data-ttu-id="7056e-110">Date</span><span class="sxs-lookup"><span data-stu-id="7056e-110">Date</span></span>| <span data-ttu-id="7056e-111">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="7056e-111">Birth date of the student.</span></span>|
|<span data-ttu-id="7056e-112">externalId</span><span class="sxs-lookup"><span data-stu-id="7056e-112">externalId</span></span>|<span data-ttu-id="7056e-113">String</span><span class="sxs-lookup"><span data-stu-id="7056e-113">String</span></span>| <span data-ttu-id="7056e-114">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="7056e-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="7056e-115">gender</span><span class="sxs-lookup"><span data-stu-id="7056e-115">gender</span></span>|<span data-ttu-id="7056e-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="7056e-116">educationGender</span></span>| <span data-ttu-id="7056e-117">Die möglichen Werte sind: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7056e-117">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7056e-118">grade</span><span class="sxs-lookup"><span data-stu-id="7056e-118">grade</span></span>|<span data-ttu-id="7056e-119">String</span><span class="sxs-lookup"><span data-stu-id="7056e-119">String</span></span>|<span data-ttu-id="7056e-120">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="7056e-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="7056e-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="7056e-121">graduationYear</span></span>|<span data-ttu-id="7056e-122">String</span><span class="sxs-lookup"><span data-stu-id="7056e-122">String</span></span>| <span data-ttu-id="7056e-123">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="7056e-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="7056e-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="7056e-124">studentNumber</span></span>|<span data-ttu-id="7056e-125">String</span><span class="sxs-lookup"><span data-stu-id="7056e-125">String</span></span>| <span data-ttu-id="7056e-126">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="7056e-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7056e-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7056e-127">JSON representation</span></span>

<span data-ttu-id="7056e-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7056e-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
