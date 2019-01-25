---
title: Ressourcentyp bookingCustomer
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522217"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="80d8b-104">Ressourcentyp bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="80d8b-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="80d8b-105">Stellt ein Kunde von einer [BookingBsiness](bookingbusiness.md)dar.</span><span class="sxs-lookup"><span data-stu-id="80d8b-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="80d8b-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="80d8b-106">Methods</span></span>

| <span data-ttu-id="80d8b-107">Methode</span><span class="sxs-lookup"><span data-stu-id="80d8b-107">Method</span></span>           | <span data-ttu-id="80d8b-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="80d8b-108">Return Type</span></span>    |<span data-ttu-id="80d8b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80d8b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80d8b-110">Liste von Kunden</span><span class="sxs-lookup"><span data-stu-id="80d8b-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="80d8b-111">[BookingCustomer](bookingcustomer.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="80d8b-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="80d8b-112">Abrufen einer Liste von **BookingCustomer** -Objekten.</span><span class="sxs-lookup"><span data-stu-id="80d8b-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="80d8b-113">Erstellen von bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="80d8b-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="80d8b-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="80d8b-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="80d8b-115">Erstellen eines neuen **BookingCustomer** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="80d8b-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="80d8b-116">Abrufen von bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="80d8b-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="80d8b-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="80d8b-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="80d8b-118">Lesen Sie die Eigenschaften und die Beziehungen eines **BookingCustomer** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="80d8b-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="80d8b-119">Update</span><span class="sxs-lookup"><span data-stu-id="80d8b-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="80d8b-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="80d8b-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="80d8b-121">Aktualisieren eines **BookingCustomer** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="80d8b-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="80d8b-122">Delete</span><span class="sxs-lookup"><span data-stu-id="80d8b-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="80d8b-123">Keine</span><span class="sxs-lookup"><span data-stu-id="80d8b-123">None</span></span> |<span data-ttu-id="80d8b-124">Löscht ein Objekt **BookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="80d8b-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80d8b-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80d8b-125">Properties</span></span>
| <span data-ttu-id="80d8b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80d8b-126">Property</span></span>     | <span data-ttu-id="80d8b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="80d8b-127">Type</span></span>   |<span data-ttu-id="80d8b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80d8b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80d8b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="80d8b-129">displayName</span></span>|<span data-ttu-id="80d8b-130">String</span><span class="sxs-lookup"><span data-stu-id="80d8b-130">String</span></span>|<span data-ttu-id="80d8b-131">Der Name des Kunden.</span><span class="sxs-lookup"><span data-stu-id="80d8b-131">The name of the customer.</span></span>|
|<span data-ttu-id="80d8b-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="80d8b-132">emailAddress</span></span>|<span data-ttu-id="80d8b-133">String</span><span class="sxs-lookup"><span data-stu-id="80d8b-133">String</span></span>|<span data-ttu-id="80d8b-134">Die SMTP-Adresse des Kunden.</span><span class="sxs-lookup"><span data-stu-id="80d8b-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="80d8b-135">id</span><span class="sxs-lookup"><span data-stu-id="80d8b-135">id</span></span>|<span data-ttu-id="80d8b-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80d8b-136">String</span></span>| <span data-ttu-id="80d8b-137">Die ID des Kunden.</span><span class="sxs-lookup"><span data-stu-id="80d8b-137">The ID of the customer.</span></span> <span data-ttu-id="80d8b-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80d8b-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80d8b-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="80d8b-139">Relationships</span></span>
<span data-ttu-id="80d8b-140">Keine</span><span class="sxs-lookup"><span data-stu-id="80d8b-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="80d8b-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80d8b-141">JSON representation</span></span>

<span data-ttu-id="80d8b-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80d8b-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
