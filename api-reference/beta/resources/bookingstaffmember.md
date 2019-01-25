---
title: Ressourcentyp bookingStaffMember
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520277"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="8df36-104">Ressourcentyp bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8df36-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="8df36-105">Stellt ein Mitarbeiter, die in einer [BookingBusiness](bookingbusiness.md)-Dienste bietet.</span><span class="sxs-lookup"><span data-stu-id="8df36-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="8df36-106">Mitarbeiter können Teil des Office-355 Mandanten sein, auf dem das Buchen Unternehmen konfiguriert ist, oder sie können e-Mail-Dienste von anderen e-Mail-Anbietern.</span><span class="sxs-lookup"><span data-stu-id="8df36-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="8df36-107">Beim Buchen von Terminen berücksichtigt die Buchungen API die folgenden Einstellungen, um ein Mitarbeiter Verfügbarkeit zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="8df36-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="8df36-108">In der Standardeinstellung stellt den Betriebszeiten des Unternehmens (die **BusinessHours** -Eigenschaft der Entität [BookingBusiness](bookingbusiness.md) ) die allgemeine Verfügbarkeit des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="8df36-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="8df36-109">Wenn **UseBusinessHours** auf false festgelegt ist, stellt der Mitarbeiter bestimmte Arbeitsstunden (**WorkingHours** -Eigenschaft der Entität **BookingStaffmember** ) allgemeine Verfügbarkeit des Mitglieds an.</span><span class="sxs-lookup"><span data-stu-id="8df36-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="8df36-110">Wenn **AvailabilityIsAffectedByPersonalCalendar** auf true festgelegt ist, klicken Sie dann die Buchungen API würde zunächst sehen Sie sich die Mitarbeiter im Allgemeinen verfügbaren Stunden (wie von #1 oder 2 # bestimmt), und überprüfen Sie die Verfügbarkeit während der Stunden, die in der Mitarbeiter persönlich vor der Durchführung einer buchen Kalender.</span><span class="sxs-lookup"><span data-stu-id="8df36-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="8df36-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="8df36-111">Methods</span></span>

| <span data-ttu-id="8df36-112">Methode</span><span class="sxs-lookup"><span data-stu-id="8df36-112">Method</span></span>           | <span data-ttu-id="8df36-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8df36-113">Return Type</span></span>    |<span data-ttu-id="8df36-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8df36-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8df36-115">Liste Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="8df36-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="8df36-116">[BookingStaffMember](bookingstaffmember.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8df36-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="8df36-117">Rufen Sie eine Liste der **BookingStaffMember** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8df36-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="8df36-118">Erstellen von bookingStaff</span><span class="sxs-lookup"><span data-stu-id="8df36-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="8df36-119">[BookingStaffMember](bookingstaffmember.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8df36-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="8df36-120">Erstellen Sie eine neue **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8df36-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="8df36-121">Abrufen von bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8df36-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="8df36-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8df36-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="8df36-123">Rufen Sie die Eigenschaften und Beziehungen zwischen einer **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8df36-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="8df36-124">Update</span><span class="sxs-lookup"><span data-stu-id="8df36-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="8df36-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8df36-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="8df36-126">Aktualisieren Sie die Eigenschaften einer **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8df36-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="8df36-127">Delete</span><span class="sxs-lookup"><span data-stu-id="8df36-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="8df36-128">Keine</span><span class="sxs-lookup"><span data-stu-id="8df36-128">None</span></span> |<span data-ttu-id="8df36-129">Löschen von Mitarbeitern in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8df36-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="8df36-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8df36-130">Properties</span></span>
| <span data-ttu-id="8df36-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8df36-131">Property</span></span>     | <span data-ttu-id="8df36-132">Typ</span><span class="sxs-lookup"><span data-stu-id="8df36-132">Type</span></span>   |<span data-ttu-id="8df36-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8df36-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8df36-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="8df36-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="8df36-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8df36-135">Boolean</span></span>|<span data-ttu-id="8df36-136">"True" bedeutet, dass, wenn der Mitarbeiter Office 365-Benutzer ist, der API Buchungen Verfügbarkeit der Mitarbeiter in ihre persönlichen Kalender auf Office 365, vergewissern Sie sich würde vor der Durchführung einer buchen.</span><span class="sxs-lookup"><span data-stu-id="8df36-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="8df36-137">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="8df36-137">colorIndex</span></span>|<span data-ttu-id="8df36-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8df36-138">Int32</span></span>|<span data-ttu-id="8df36-139">Identifiziert eine Farbe, um die Mitarbeiter darstellen.</span><span class="sxs-lookup"><span data-stu-id="8df36-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="8df36-140">Die Farbe entspricht der Farbpalette in der Detailseite für **Mitarbeiter** in der app Buchungen.</span><span class="sxs-lookup"><span data-stu-id="8df36-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="8df36-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8df36-141">displayName</span></span>|<span data-ttu-id="8df36-142">String</span><span class="sxs-lookup"><span data-stu-id="8df36-142">String</span></span>|<span data-ttu-id="8df36-143">Der Name des Mitarbeiters, wie Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8df36-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="8df36-144">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8df36-144">Required.</span></span>|
|<span data-ttu-id="8df36-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8df36-145">emailAddress</span></span>|<span data-ttu-id="8df36-146">String</span><span class="sxs-lookup"><span data-stu-id="8df36-146">String</span></span>|<span data-ttu-id="8df36-147">Die e-Mail-Adresse des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="8df36-147">The email address of the staff member.</span></span> <span data-ttu-id="8df36-148">Dies kann in der gleichen Office 365-Mandanten als das Unternehmen oder in eine andere e-Mail-Domäne sein.</span><span class="sxs-lookup"><span data-stu-id="8df36-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="8df36-149">Diese e-Mail-Adresse kann verwendet werden, wenn die **SendConfirmationsToOwner** -Eigenschaft festgelegt ist, auf "true" in der scheduling Richtlinie des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="8df36-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="8df36-150">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8df36-150">Required.</span></span>|
|<span data-ttu-id="8df36-151">id</span><span class="sxs-lookup"><span data-stu-id="8df36-151">id</span></span>|<span data-ttu-id="8df36-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8df36-152">String</span></span>| <span data-ttu-id="8df36-153">Die ID des Members Mitarbeiter in einer GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="8df36-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="8df36-154">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8df36-154">Read-only.</span></span>|
|<span data-ttu-id="8df36-155">role</span><span class="sxs-lookup"><span data-stu-id="8df36-155">role</span></span>|<span data-ttu-id="8df36-156">string</span><span class="sxs-lookup"><span data-stu-id="8df36-156">string</span></span>| <span data-ttu-id="8df36-157">Die Rolle des Mitarbeiters im Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="8df36-157">The role of the staff member in the business.</span></span> <span data-ttu-id="8df36-158">Mögliche Werte: sind `guest`, `administrator`, `viewer` und `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="8df36-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="8df36-159">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8df36-159">Required.</span></span>|
|<span data-ttu-id="8df36-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="8df36-160">useBusinessHours</span></span>|<span data-ttu-id="8df36-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8df36-161">Boolean</span></span>|<span data-ttu-id="8df36-162">"True" bedeutet, dass die Mitarbeiter die Verfügbarkeit als ist in der **BusinessHours** -Eigenschaft des Unternehmens angegeben.</span><span class="sxs-lookup"><span data-stu-id="8df36-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="8df36-163">False bedeutet, dass die Verfügbarkeit durch die Einstellung für die Mitarbeiter **WorkingHours** -Eigenschaft bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="8df36-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="8df36-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="8df36-164">workingHours</span></span>|<span data-ttu-id="8df36-165">[BookingWorkHours](bookingworkhours.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8df36-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="8df36-166">Der Bereich der Stunden jeden Tag der Woche, die der Mitarbeiter für buchen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="8df36-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="8df36-167">Standardmäßig werden sie initialisiert, um die **BusinessHours** -Eigenschaft des Unternehmens identisch sein.</span><span class="sxs-lookup"><span data-stu-id="8df36-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8df36-168">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8df36-168">Relationships</span></span>
<span data-ttu-id="8df36-169">Keine</span><span class="sxs-lookup"><span data-stu-id="8df36-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8df36-170">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8df36-170">JSON representation</span></span>

<span data-ttu-id="8df36-171">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8df36-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
