---
title: WorksheetProtection-Ressourcentyp
description: Stellt den Schutz eines Arbeitsblattobjekts dar.
author: lumine2008
ms.openlocfilehash: 3df3ea522b7d4f476bf09173ed7998e62e9562d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344289"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="d55ff-103">WorksheetProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d55ff-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="d55ff-104">Stellt den Schutz eines Arbeitsblattobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="d55ff-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="d55ff-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d55ff-105">Methods</span></span>

| <span data-ttu-id="d55ff-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d55ff-106">Method</span></span>           | <span data-ttu-id="d55ff-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d55ff-107">Return Type</span></span>    |<span data-ttu-id="d55ff-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d55ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d55ff-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d55ff-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="d55ff-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d55ff-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="d55ff-111">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d55ff-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="d55ff-112">Protect</span><span class="sxs-lookup"><span data-stu-id="d55ff-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="d55ff-113">Keine</span><span class="sxs-lookup"><span data-stu-id="d55ff-113">None</span></span>|<span data-ttu-id="d55ff-p101">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="d55ff-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="d55ff-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="d55ff-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="d55ff-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d55ff-117">None</span></span>|<span data-ttu-id="d55ff-118">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="d55ff-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="d55ff-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d55ff-119">Properties</span></span>
| <span data-ttu-id="d55ff-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d55ff-120">Property</span></span>     | <span data-ttu-id="d55ff-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d55ff-121">Type</span></span>   |<span data-ttu-id="d55ff-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d55ff-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d55ff-123">options</span><span class="sxs-lookup"><span data-stu-id="d55ff-123">options</span></span>|[<span data-ttu-id="d55ff-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d55ff-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="d55ff-p102">Optionen für den Arbeitsblattschutz. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d55ff-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="d55ff-127">geschützt</span><span class="sxs-lookup"><span data-stu-id="d55ff-127">protected</span></span>|<span data-ttu-id="d55ff-128">boolean</span><span class="sxs-lookup"><span data-stu-id="d55ff-128">boolean</span></span>|<span data-ttu-id="d55ff-p103">Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d55ff-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d55ff-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d55ff-131">JSON representation</span></span>

<span data-ttu-id="d55ff-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d55ff-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->