---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
ms.openlocfilehash: ce84c9f6abb71e99bf3d886e5bad9e7e97bcb513
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313083"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="2a898-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2a898-103">educationStudent resource type</span></span>

> <span data-ttu-id="2a898-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a898-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a898-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a898-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a898-106">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="2a898-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="2a898-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a898-107">Properties</span></span>
| <span data-ttu-id="2a898-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a898-108">Property</span></span>     | <span data-ttu-id="2a898-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2a898-109">Type</span></span>   |<span data-ttu-id="2a898-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a898-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a898-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="2a898-111">birthDate</span></span>|<span data-ttu-id="2a898-112">Date</span><span class="sxs-lookup"><span data-stu-id="2a898-112">Date</span></span>| <span data-ttu-id="2a898-113">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="2a898-113">Birth date of the student.</span></span>|
|<span data-ttu-id="2a898-114">externalId</span><span class="sxs-lookup"><span data-stu-id="2a898-114">externalId</span></span>|<span data-ttu-id="2a898-115">String</span><span class="sxs-lookup"><span data-stu-id="2a898-115">String</span></span>| <span data-ttu-id="2a898-116">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="2a898-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="2a898-117">gender</span><span class="sxs-lookup"><span data-stu-id="2a898-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="2a898-118">Mögliche Werte: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2a898-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="2a898-119">grade</span><span class="sxs-lookup"><span data-stu-id="2a898-119">grade</span></span>|<span data-ttu-id="2a898-120">String</span><span class="sxs-lookup"><span data-stu-id="2a898-120">String</span></span>|<span data-ttu-id="2a898-121">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="2a898-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="2a898-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="2a898-122">graduationYear</span></span>|<span data-ttu-id="2a898-123">String</span><span class="sxs-lookup"><span data-stu-id="2a898-123">String</span></span>| <span data-ttu-id="2a898-124">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="2a898-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="2a898-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="2a898-125">studentNumber</span></span>|<span data-ttu-id="2a898-126">String</span><span class="sxs-lookup"><span data-stu-id="2a898-126">String</span></span>| <span data-ttu-id="2a898-127">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="2a898-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a898-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a898-128">JSON representation</span></span>

<span data-ttu-id="2a898-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a898-129">The following is a JSON representation of the resource.</span></span>

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