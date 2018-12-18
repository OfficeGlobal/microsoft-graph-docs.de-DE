---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
ms.openlocfilehash: e24cf9adb9a4e7da70a3011b027e19a9d4cc4808
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344058"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="177f2-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="177f2-103">educationStudent resource type</span></span>

<span data-ttu-id="177f2-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="177f2-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="177f2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="177f2-105">Properties</span></span>
| <span data-ttu-id="177f2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="177f2-106">Property</span></span>     | <span data-ttu-id="177f2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="177f2-107">Type</span></span>   |<span data-ttu-id="177f2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="177f2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="177f2-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="177f2-109">birthDate</span></span>|<span data-ttu-id="177f2-110">Date</span><span class="sxs-lookup"><span data-stu-id="177f2-110">Date</span></span>| <span data-ttu-id="177f2-111">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="177f2-111">Birth date of the student.</span></span>|
|<span data-ttu-id="177f2-112">externalId</span><span class="sxs-lookup"><span data-stu-id="177f2-112">externalId</span></span>|<span data-ttu-id="177f2-113">String</span><span class="sxs-lookup"><span data-stu-id="177f2-113">String</span></span>| <span data-ttu-id="177f2-114">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="177f2-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="177f2-115">gender</span><span class="sxs-lookup"><span data-stu-id="177f2-115">gender</span></span>|<span data-ttu-id="177f2-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="177f2-116">educationGender</span></span>| <span data-ttu-id="177f2-117">Die möglichen Werte sind: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="177f2-117">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="177f2-118">grade</span><span class="sxs-lookup"><span data-stu-id="177f2-118">grade</span></span>|<span data-ttu-id="177f2-119">String</span><span class="sxs-lookup"><span data-stu-id="177f2-119">String</span></span>|<span data-ttu-id="177f2-120">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="177f2-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="177f2-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="177f2-121">graduationYear</span></span>|<span data-ttu-id="177f2-122">String</span><span class="sxs-lookup"><span data-stu-id="177f2-122">String</span></span>| <span data-ttu-id="177f2-123">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="177f2-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="177f2-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="177f2-124">studentNumber</span></span>|<span data-ttu-id="177f2-125">String</span><span class="sxs-lookup"><span data-stu-id="177f2-125">String</span></span>| <span data-ttu-id="177f2-126">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="177f2-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="177f2-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="177f2-127">JSON representation</span></span>

<span data-ttu-id="177f2-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="177f2-128">The following is a JSON representation of the resource.</span></span>

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
