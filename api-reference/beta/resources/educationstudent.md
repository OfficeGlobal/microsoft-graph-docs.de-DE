---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b6f6cf8e8a79c427403c2f2157228c8ce130b313
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913310"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="a1978-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1978-103">educationStudent resource type</span></span>

> <span data-ttu-id="a1978-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a1978-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1978-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1978-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1978-106">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="a1978-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="a1978-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1978-107">Properties</span></span>
| <span data-ttu-id="a1978-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1978-108">Property</span></span>     | <span data-ttu-id="a1978-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a1978-109">Type</span></span>   |<span data-ttu-id="a1978-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1978-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1978-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="a1978-111">birthDate</span></span>|<span data-ttu-id="a1978-112">Date</span><span class="sxs-lookup"><span data-stu-id="a1978-112">Date</span></span>| <span data-ttu-id="a1978-113">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a1978-113">Birth date of the student.</span></span>|
|<span data-ttu-id="a1978-114">externalId</span><span class="sxs-lookup"><span data-stu-id="a1978-114">externalId</span></span>|<span data-ttu-id="a1978-115">String</span><span class="sxs-lookup"><span data-stu-id="a1978-115">String</span></span>| <span data-ttu-id="a1978-116">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="a1978-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="a1978-117">gender</span><span class="sxs-lookup"><span data-stu-id="a1978-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="a1978-118">Mögliche Werte: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a1978-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="a1978-119">grade</span><span class="sxs-lookup"><span data-stu-id="a1978-119">grade</span></span>|<span data-ttu-id="a1978-120">String</span><span class="sxs-lookup"><span data-stu-id="a1978-120">String</span></span>|<span data-ttu-id="a1978-121">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a1978-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="a1978-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="a1978-122">graduationYear</span></span>|<span data-ttu-id="a1978-123">String</span><span class="sxs-lookup"><span data-stu-id="a1978-123">String</span></span>| <span data-ttu-id="a1978-124">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="a1978-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="a1978-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="a1978-125">studentNumber</span></span>|<span data-ttu-id="a1978-126">String</span><span class="sxs-lookup"><span data-stu-id="a1978-126">String</span></span>| <span data-ttu-id="a1978-127">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="a1978-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1978-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1978-128">JSON representation</span></span>

<span data-ttu-id="a1978-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1978-129">The following is a JSON representation of the resource.</span></span>

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
