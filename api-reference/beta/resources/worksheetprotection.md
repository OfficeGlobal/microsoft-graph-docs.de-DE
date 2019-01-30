---
title: WorksheetProtection-Ressourcentyp
description: Stellt den Schutz eines Arbeitsblattobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29639944"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="af4cf-103">WorksheetProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="af4cf-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af4cf-104">Stellt den Schutz eines Arbeitsblattobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="af4cf-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="af4cf-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="af4cf-105">Methods</span></span>

| <span data-ttu-id="af4cf-106">Methode</span><span class="sxs-lookup"><span data-stu-id="af4cf-106">Method</span></span>           | <span data-ttu-id="af4cf-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="af4cf-107">Return Type</span></span>    |<span data-ttu-id="af4cf-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af4cf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af4cf-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="af4cf-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="af4cf-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="af4cf-110">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="af4cf-111">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="af4cf-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="af4cf-112">Protect</span><span class="sxs-lookup"><span data-stu-id="af4cf-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="af4cf-113">Keine</span><span class="sxs-lookup"><span data-stu-id="af4cf-113">None</span></span>|<span data-ttu-id="af4cf-p101">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="af4cf-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="af4cf-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="af4cf-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="af4cf-117">Keine</span><span class="sxs-lookup"><span data-stu-id="af4cf-117">None</span></span>|<span data-ttu-id="af4cf-118">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="af4cf-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="af4cf-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="af4cf-119">Properties</span></span>
| <span data-ttu-id="af4cf-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af4cf-120">Property</span></span>     | <span data-ttu-id="af4cf-121">Typ</span><span class="sxs-lookup"><span data-stu-id="af4cf-121">Type</span></span>   |<span data-ttu-id="af4cf-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af4cf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af4cf-123">geschützt</span><span class="sxs-lookup"><span data-stu-id="af4cf-123">protected</span></span>|<span data-ttu-id="af4cf-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="af4cf-124">boolean</span></span>|<span data-ttu-id="af4cf-p102">Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="af4cf-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af4cf-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="af4cf-127">Relationships</span></span>
| <span data-ttu-id="af4cf-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="af4cf-128">Relationship</span></span> | <span data-ttu-id="af4cf-129">Typ</span><span class="sxs-lookup"><span data-stu-id="af4cf-129">Type</span></span>   |<span data-ttu-id="af4cf-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af4cf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af4cf-131">options</span><span class="sxs-lookup"><span data-stu-id="af4cf-131">options</span></span>|[<span data-ttu-id="af4cf-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="af4cf-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="af4cf-p103">Optionen für den Arbeitsblattschutz. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="af4cf-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af4cf-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="af4cf-135">JSON representation</span></span>

<span data-ttu-id="af4cf-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="af4cf-136">Here is a JSON representation of the resource.</span></span>

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
