---
title: WorksheetProtection-Ressourcentyp
description: Stellt den Schutz eines Arbeitsblattobjekts dar.
author: lumine2008
ms.openlocfilehash: 91415b067fbe54333e32d1a2ed84bce5025b7d3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339207"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="4949c-103">WorksheetProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4949c-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="4949c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4949c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4949c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4949c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4949c-106">Stellt den Schutz eines Arbeitsblattobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="4949c-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4949c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="4949c-107">Methods</span></span>

| <span data-ttu-id="4949c-108">Methode</span><span class="sxs-lookup"><span data-stu-id="4949c-108">Method</span></span>           | <span data-ttu-id="4949c-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4949c-109">Return Type</span></span>    |<span data-ttu-id="4949c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4949c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4949c-111">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4949c-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="4949c-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4949c-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="4949c-113">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4949c-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="4949c-114">Protect</span><span class="sxs-lookup"><span data-stu-id="4949c-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="4949c-115">Keine</span><span class="sxs-lookup"><span data-stu-id="4949c-115">None</span></span>|<span data-ttu-id="4949c-p102">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="4949c-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4949c-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="4949c-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="4949c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="4949c-119">None</span></span>|<span data-ttu-id="4949c-120">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="4949c-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4949c-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4949c-121">Properties</span></span>
| <span data-ttu-id="4949c-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4949c-122">Property</span></span>     | <span data-ttu-id="4949c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="4949c-123">Type</span></span>   |<span data-ttu-id="4949c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4949c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4949c-125">geschützt</span><span class="sxs-lookup"><span data-stu-id="4949c-125">protected</span></span>|<span data-ttu-id="4949c-126">boolean</span><span class="sxs-lookup"><span data-stu-id="4949c-126">boolean</span></span>|<span data-ttu-id="4949c-p103">Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4949c-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4949c-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4949c-129">Relationships</span></span>
| <span data-ttu-id="4949c-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4949c-130">Relationship</span></span> | <span data-ttu-id="4949c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4949c-131">Type</span></span>   |<span data-ttu-id="4949c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4949c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4949c-133">options</span><span class="sxs-lookup"><span data-stu-id="4949c-133">options</span></span>|[<span data-ttu-id="4949c-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4949c-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="4949c-p104">Optionen für den Arbeitsblattschutz. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4949c-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4949c-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4949c-137">JSON representation</span></span>

<span data-ttu-id="4949c-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4949c-138">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->