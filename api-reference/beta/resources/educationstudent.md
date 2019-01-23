---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ce3e28ccedc5f6165c8c333afb2ccd10343f14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406906"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="d66d2-103">educationStudent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d66d2-103">educationStudent resource type</span></span>

> <span data-ttu-id="d66d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d66d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d66d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d66d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d66d2-106">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.</span><span class="sxs-lookup"><span data-stu-id="d66d2-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="d66d2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d66d2-107">Properties</span></span>
| <span data-ttu-id="d66d2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d66d2-108">Property</span></span>     | <span data-ttu-id="d66d2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d66d2-109">Type</span></span>   |<span data-ttu-id="d66d2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d66d2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d66d2-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="d66d2-111">birthDate</span></span>|<span data-ttu-id="d66d2-112">Date</span><span class="sxs-lookup"><span data-stu-id="d66d2-112">Date</span></span>| <span data-ttu-id="d66d2-113">Geburtsdatum des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="d66d2-113">Birth date of the student.</span></span>|
|<span data-ttu-id="d66d2-114">externalId</span><span class="sxs-lookup"><span data-stu-id="d66d2-114">externalId</span></span>|<span data-ttu-id="d66d2-115">String</span><span class="sxs-lookup"><span data-stu-id="d66d2-115">String</span></span>| <span data-ttu-id="d66d2-116">ID des Kursteilnehmers im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="d66d2-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="d66d2-117">gender</span><span class="sxs-lookup"><span data-stu-id="d66d2-117">gender</span></span>|<span data-ttu-id="d66d2-118">educationGender</span><span class="sxs-lookup"><span data-stu-id="d66d2-118">educationGender</span></span>| <span data-ttu-id="d66d2-119">Mögliche Werte: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d66d2-119">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="d66d2-120">grade</span><span class="sxs-lookup"><span data-stu-id="d66d2-120">grade</span></span>|<span data-ttu-id="d66d2-121">String</span><span class="sxs-lookup"><span data-stu-id="d66d2-121">String</span></span>|<span data-ttu-id="d66d2-122">Aktuelle Klassenstufe des Kursteilnehmers.</span><span class="sxs-lookup"><span data-stu-id="d66d2-122">Current grade level of the student.</span></span>|
|<span data-ttu-id="d66d2-123">graduationYear</span><span class="sxs-lookup"><span data-stu-id="d66d2-123">graduationYear</span></span>|<span data-ttu-id="d66d2-124">String</span><span class="sxs-lookup"><span data-stu-id="d66d2-124">String</span></span>| <span data-ttu-id="d66d2-125">Jahr, in dem der Kursteilnehmer die Schule abschließt.</span><span class="sxs-lookup"><span data-stu-id="d66d2-125">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="d66d2-126">studentNumber</span><span class="sxs-lookup"><span data-stu-id="d66d2-126">studentNumber</span></span>|<span data-ttu-id="d66d2-127">String</span><span class="sxs-lookup"><span data-stu-id="d66d2-127">String</span></span>| <span data-ttu-id="d66d2-128">Kursteilnehmernummer</span><span class="sxs-lookup"><span data-stu-id="d66d2-128">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d66d2-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d66d2-129">JSON representation</span></span>

<span data-ttu-id="d66d2-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d66d2-130">The following is a JSON representation of the resource.</span></span>

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
