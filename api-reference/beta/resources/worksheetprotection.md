---
title: WorksheetProtection-Ressourcentyp
description: Stellt den Schutz eines Arbeitsblattobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512038"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="d738b-103">WorksheetProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d738b-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d738b-104">Stellt den Schutz eines Arbeitsblattobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="d738b-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="d738b-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d738b-105">Methods</span></span>

| <span data-ttu-id="d738b-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d738b-106">Method</span></span>           | <span data-ttu-id="d738b-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d738b-107">Return Type</span></span>    |<span data-ttu-id="d738b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d738b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d738b-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d738b-109">[Get WorksheetProtection](../api/worksheetprotection-get.md)</span></span> | <span data-ttu-id="d738b-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d738b-110">[WorksheetProtection](worksheetprotection.md)</span></span> |<span data-ttu-id="d738b-111">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d738b-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="d738b-112">Protect</span><span class="sxs-lookup"><span data-stu-id="d738b-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="d738b-113">Keine</span><span class="sxs-lookup"><span data-stu-id="d738b-113">None</span></span>|<span data-ttu-id="d738b-p101">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="d738b-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="d738b-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="d738b-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="d738b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d738b-117">None</span></span>|<span data-ttu-id="d738b-118">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="d738b-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="d738b-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d738b-119">Properties</span></span>
| <span data-ttu-id="d738b-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d738b-120">Property</span></span>     | <span data-ttu-id="d738b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d738b-121">Type</span></span>   |<span data-ttu-id="d738b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d738b-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d738b-123">geschützt</span><span class="sxs-lookup"><span data-stu-id="d738b-123">protected</span></span>|<span data-ttu-id="d738b-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d738b-124">boolean</span></span>|<span data-ttu-id="d738b-p102">Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d738b-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d738b-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d738b-127">Relationships</span></span>
| <span data-ttu-id="d738b-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d738b-128">Relationship</span></span> | <span data-ttu-id="d738b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d738b-129">Type</span></span>   |<span data-ttu-id="d738b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d738b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d738b-131">options</span><span class="sxs-lookup"><span data-stu-id="d738b-131">options</span></span>|[<span data-ttu-id="d738b-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d738b-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="d738b-p103">Optionen für den Arbeitsblattschutz. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d738b-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d738b-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d738b-135">JSON representation</span></span>

<span data-ttu-id="d738b-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d738b-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
