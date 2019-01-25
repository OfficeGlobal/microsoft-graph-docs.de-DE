---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen `student` hinzugefügt werden, wenn die primaryRole eines Benutzers  ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522035"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="41c9d-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="41c9d-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41c9d-104">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="41c9d-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="41c9d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41c9d-105">Properties</span></span>
| <span data-ttu-id="41c9d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41c9d-106">Property</span></span>     | <span data-ttu-id="41c9d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="41c9d-107">Type</span></span>   |<span data-ttu-id="41c9d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41c9d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41c9d-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="41c9d-109">birthDate</span></span>|<span data-ttu-id="41c9d-110">Date</span><span class="sxs-lookup"><span data-stu-id="41c9d-110">Date</span></span>| <span data-ttu-id="41c9d-111">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="41c9d-111">Birth date of the student.</span></span>|
|<span data-ttu-id="41c9d-112">externalId</span><span class="sxs-lookup"><span data-stu-id="41c9d-112">externalId</span></span>|<span data-ttu-id="41c9d-113">String</span><span class="sxs-lookup"><span data-stu-id="41c9d-113">String</span></span>| <span data-ttu-id="41c9d-114">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="41c9d-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="41c9d-115">gender</span><span class="sxs-lookup"><span data-stu-id="41c9d-115">gender</span></span>|<span data-ttu-id="41c9d-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="41c9d-116">educationGender</span></span>| <span data-ttu-id="41c9d-117">Mögliche Werte: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="41c9d-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="41c9d-118">grade</span><span class="sxs-lookup"><span data-stu-id="41c9d-118">grade</span></span>|<span data-ttu-id="41c9d-119">String</span><span class="sxs-lookup"><span data-stu-id="41c9d-119">String</span></span>|<span data-ttu-id="41c9d-120">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="41c9d-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="41c9d-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="41c9d-121">graduationYear</span></span>|<span data-ttu-id="41c9d-122">String</span><span class="sxs-lookup"><span data-stu-id="41c9d-122">String</span></span>| <span data-ttu-id="41c9d-123">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="41c9d-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="41c9d-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="41c9d-124">studentNumber</span></span>|<span data-ttu-id="41c9d-125">String</span><span class="sxs-lookup"><span data-stu-id="41c9d-125">String</span></span>| <span data-ttu-id="41c9d-126">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="41c9d-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41c9d-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41c9d-127">JSON representation</span></span>

<span data-ttu-id="41c9d-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41c9d-128">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationstudent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
