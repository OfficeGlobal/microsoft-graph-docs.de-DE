---
title: WorksheetProtection-Ressourcentyp
description: Stellt den Schutz eines Arbeitsblattobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6f32ad7b1cc25d9a937f2de68f1bd930d92ec8f9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572934"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="370e2-103">WorksheetProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="370e2-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="370e2-104">Stellt den Schutz eines Arbeitsblattobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="370e2-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="370e2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="370e2-105">Methods</span></span>

| <span data-ttu-id="370e2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="370e2-106">Method</span></span>           | <span data-ttu-id="370e2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="370e2-107">Return Type</span></span>    |<span data-ttu-id="370e2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="370e2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="370e2-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="370e2-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="370e2-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="370e2-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="370e2-111">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="370e2-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="370e2-112">Protect</span><span class="sxs-lookup"><span data-stu-id="370e2-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="370e2-113">Keine</span><span class="sxs-lookup"><span data-stu-id="370e2-113">None</span></span>|<span data-ttu-id="370e2-p101">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="370e2-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="370e2-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="370e2-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="370e2-117">Keine</span><span class="sxs-lookup"><span data-stu-id="370e2-117">None</span></span>|<span data-ttu-id="370e2-118">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="370e2-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="370e2-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="370e2-119">Properties</span></span>
| <span data-ttu-id="370e2-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="370e2-120">Property</span></span>     | <span data-ttu-id="370e2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="370e2-121">Type</span></span>   |<span data-ttu-id="370e2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="370e2-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="370e2-123">geschützt</span><span class="sxs-lookup"><span data-stu-id="370e2-123">protected</span></span>|<span data-ttu-id="370e2-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="370e2-124">boolean</span></span>|<span data-ttu-id="370e2-p102">Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="370e2-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="370e2-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="370e2-127">Relationships</span></span>
| <span data-ttu-id="370e2-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="370e2-128">Relationship</span></span> | <span data-ttu-id="370e2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="370e2-129">Type</span></span>   |<span data-ttu-id="370e2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="370e2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="370e2-131">options</span><span class="sxs-lookup"><span data-stu-id="370e2-131">options</span></span>|[<span data-ttu-id="370e2-132">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="370e2-132">workbookWorksheetProtection</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="370e2-p103">Optionen für den Arbeitsblattschutz. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="370e2-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="370e2-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="370e2-135">JSON representation</span></span>

<span data-ttu-id="370e2-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="370e2-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "options"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
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
