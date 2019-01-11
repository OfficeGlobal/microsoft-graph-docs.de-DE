---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 80135827abb2dbf934e7ebec5e25ae6a52e58513
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822050"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="42a6b-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="42a6b-103">educationStudent resource type</span></span>

<span data-ttu-id="42a6b-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="42a6b-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="42a6b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42a6b-105">Properties</span></span>
| <span data-ttu-id="42a6b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42a6b-106">Property</span></span>     | <span data-ttu-id="42a6b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="42a6b-107">Type</span></span>   |<span data-ttu-id="42a6b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42a6b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42a6b-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="42a6b-109">birthDate</span></span>|<span data-ttu-id="42a6b-110">Date</span><span class="sxs-lookup"><span data-stu-id="42a6b-110">Date</span></span>| <span data-ttu-id="42a6b-111">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="42a6b-111">Birth date of the student.</span></span>|
|<span data-ttu-id="42a6b-112">externalId</span><span class="sxs-lookup"><span data-stu-id="42a6b-112">externalId</span></span>|<span data-ttu-id="42a6b-113">String</span><span class="sxs-lookup"><span data-stu-id="42a6b-113">String</span></span>| <span data-ttu-id="42a6b-114">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="42a6b-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="42a6b-115">gender</span><span class="sxs-lookup"><span data-stu-id="42a6b-115">gender</span></span>|<span data-ttu-id="42a6b-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="42a6b-116">educationGender</span></span>| <span data-ttu-id="42a6b-117">Die möglichen Werte sind: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="42a6b-117">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="42a6b-118">grade</span><span class="sxs-lookup"><span data-stu-id="42a6b-118">grade</span></span>|<span data-ttu-id="42a6b-119">String</span><span class="sxs-lookup"><span data-stu-id="42a6b-119">String</span></span>|<span data-ttu-id="42a6b-120">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="42a6b-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="42a6b-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="42a6b-121">graduationYear</span></span>|<span data-ttu-id="42a6b-122">String</span><span class="sxs-lookup"><span data-stu-id="42a6b-122">String</span></span>| <span data-ttu-id="42a6b-123">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="42a6b-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="42a6b-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="42a6b-124">studentNumber</span></span>|<span data-ttu-id="42a6b-125">String</span><span class="sxs-lookup"><span data-stu-id="42a6b-125">String</span></span>| <span data-ttu-id="42a6b-126">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="42a6b-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42a6b-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42a6b-127">JSON representation</span></span>

<span data-ttu-id="42a6b-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42a6b-128">The following is a JSON representation of the resource.</span></span>

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
