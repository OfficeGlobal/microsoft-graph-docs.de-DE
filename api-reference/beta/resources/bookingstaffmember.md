---
title: Ressourcentyp bookingStaffMember
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 382da1b0710b691a6563a40c03ed62397262911d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884455"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="6e5b9-104">Ressourcentyp bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="6e5b9-104">bookingStaffMember resource type</span></span>

 > <span data-ttu-id="6e5b9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e5b9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6e5b9-107">Stellt ein Mitarbeiter, die in einer [BookingBusiness](bookingbusiness.md)-Dienste bietet.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-107">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="6e5b9-108">Mitarbeiter können Teil des Office-355 Mandanten sein, auf dem das Buchen Unternehmen konfiguriert ist, oder sie können e-Mail-Dienste von anderen e-Mail-Anbietern.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-108">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="6e5b9-109">Beim Buchen von Terminen berücksichtigt die Buchungen API die folgenden Einstellungen, um ein Mitarbeiter Verfügbarkeit zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="6e5b9-109">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="6e5b9-110">In der Standardeinstellung stellt den Betriebszeiten des Unternehmens (die **BusinessHours** -Eigenschaft der Entität [BookingBusiness](bookingbusiness.md) ) die allgemeine Verfügbarkeit des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-110">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="6e5b9-111">Wenn **UseBusinessHours** auf false festgelegt ist, stellt der Mitarbeiter bestimmte Arbeitsstunden (**WorkingHours** -Eigenschaft der Entität **BookingStaffmember** ) allgemeine Verfügbarkeit des Mitglieds an.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-111">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="6e5b9-112">Wenn **AvailabilityIsAffectedByPersonalCalendar** auf true festgelegt ist, klicken Sie dann die Buchungen API würde zunächst sehen Sie sich die Mitarbeiter im Allgemeinen verfügbaren Stunden (wie von #1 oder 2 # bestimmt), und überprüfen Sie die Verfügbarkeit während der Stunden, die in der Mitarbeiter persönlich vor der Durchführung einer buchen Kalender.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-112">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="6e5b9-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="6e5b9-113">Methods</span></span>

| <span data-ttu-id="6e5b9-114">Methode</span><span class="sxs-lookup"><span data-stu-id="6e5b9-114">Method</span></span>           | <span data-ttu-id="6e5b9-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6e5b9-115">Return Type</span></span>    |<span data-ttu-id="6e5b9-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e5b9-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e5b9-117">Liste Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="6e5b9-117">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="6e5b9-118">[BookingStaffMember](bookingstaffmember.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6e5b9-118">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="6e5b9-119">Rufen Sie eine Liste der **BookingStaffMember** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6e5b9-119">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="6e5b9-120">Erstellen von bookingStaff</span><span class="sxs-lookup"><span data-stu-id="6e5b9-120">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="6e5b9-121">[BookingStaffMember](bookingstaffmember.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6e5b9-121">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="6e5b9-122">Erstellen Sie eine neue **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6e5b9-122">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="6e5b9-123">Abrufen von bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="6e5b9-123">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="6e5b9-124">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="6e5b9-124">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="6e5b9-125">Rufen Sie die Eigenschaften und Beziehungen zwischen einer **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6e5b9-125">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="6e5b9-126">Update</span><span class="sxs-lookup"><span data-stu-id="6e5b9-126">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="6e5b9-127">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="6e5b9-127">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="6e5b9-128">Aktualisieren Sie die Eigenschaften einer **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6e5b9-128">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="6e5b9-129">Delete</span><span class="sxs-lookup"><span data-stu-id="6e5b9-129">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="6e5b9-130">Keine</span><span class="sxs-lookup"><span data-stu-id="6e5b9-130">None</span></span> |<span data-ttu-id="6e5b9-131">Löschen von Mitarbeitern in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6e5b9-131">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="6e5b9-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6e5b9-132">Properties</span></span>
| <span data-ttu-id="6e5b9-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6e5b9-133">Property</span></span>     | <span data-ttu-id="6e5b9-134">Typ</span><span class="sxs-lookup"><span data-stu-id="6e5b9-134">Type</span></span>   |<span data-ttu-id="6e5b9-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e5b9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e5b9-136">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="6e5b9-136">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="6e5b9-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e5b9-137">Boolean</span></span>|<span data-ttu-id="6e5b9-138">"True" bedeutet, dass, wenn der Mitarbeiter Office 365-Benutzer ist, der API Buchungen Verfügbarkeit der Mitarbeiter in ihre persönlichen Kalender auf Office 365, vergewissern Sie sich würde vor der Durchführung einer buchen.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-138">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="6e5b9-139">colorIndex</span><span class="sxs-lookup"><span data-stu-id="6e5b9-139">colorIndex</span></span>|<span data-ttu-id="6e5b9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6e5b9-140">Int32</span></span>|<span data-ttu-id="6e5b9-141">Identifiziert eine Farbe, um die Mitarbeiter darstellen.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-141">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="6e5b9-142">Die Farbe entspricht der Farbpalette in der Detailseite für **Mitarbeiter** in der app Buchungen.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-142">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="6e5b9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="6e5b9-143">displayName</span></span>|<span data-ttu-id="6e5b9-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e5b9-144">String</span></span>|<span data-ttu-id="6e5b9-145">Der Name des Mitarbeiters, wie Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-145">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="6e5b9-146">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-146">Required.</span></span>|
|<span data-ttu-id="6e5b9-147">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6e5b9-147">emailAddress</span></span>|<span data-ttu-id="6e5b9-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e5b9-148">String</span></span>|<span data-ttu-id="6e5b9-149">Die e-Mail-Adresse des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-149">The email address of the staff member.</span></span> <span data-ttu-id="6e5b9-150">Dies kann in der gleichen Office 365-Mandanten als das Unternehmen oder in eine andere e-Mail-Domäne sein.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-150">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="6e5b9-151">Diese e-Mail-Adresse kann verwendet werden, wenn die **SendConfirmationsToOwner** -Eigenschaft festgelegt ist, auf "true" in der scheduling Richtlinie des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-151">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="6e5b9-152">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-152">Required.</span></span>|
|<span data-ttu-id="6e5b9-153">id</span><span class="sxs-lookup"><span data-stu-id="6e5b9-153">id</span></span>|<span data-ttu-id="6e5b9-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e5b9-154">String</span></span>| <span data-ttu-id="6e5b9-155">Die ID des Members Mitarbeiter in einer GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-155">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="6e5b9-156">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-156">Read-only.</span></span>|
|<span data-ttu-id="6e5b9-157">role</span><span class="sxs-lookup"><span data-stu-id="6e5b9-157">role</span></span>|<span data-ttu-id="6e5b9-158">string</span><span class="sxs-lookup"><span data-stu-id="6e5b9-158">string</span></span>| <span data-ttu-id="6e5b9-159">Die Rolle des Mitarbeiters im Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-159">The role of the staff member in the business.</span></span> <span data-ttu-id="6e5b9-160">Mögliche Werte: sind `guest`, `administrator`, `viewer` und `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-160">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="6e5b9-161">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-161">Required.</span></span>|
|<span data-ttu-id="6e5b9-162">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="6e5b9-162">useBusinessHours</span></span>|<span data-ttu-id="6e5b9-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e5b9-163">Boolean</span></span>|<span data-ttu-id="6e5b9-164">"True" bedeutet, dass die Mitarbeiter die Verfügbarkeit als ist in der **BusinessHours** -Eigenschaft des Unternehmens angegeben.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-164">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="6e5b9-165">False bedeutet, dass die Verfügbarkeit durch die Einstellung für die Mitarbeiter **WorkingHours** -Eigenschaft bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-165">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="6e5b9-166">workingHours</span><span class="sxs-lookup"><span data-stu-id="6e5b9-166">workingHours</span></span>|<span data-ttu-id="6e5b9-167">[BookingWorkHours](bookingworkhours.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6e5b9-167">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="6e5b9-168">Der Bereich der Stunden jeden Tag der Woche, die der Mitarbeiter für buchen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-168">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="6e5b9-169">Standardmäßig werden sie initialisiert, um die **BusinessHours** -Eigenschaft des Unternehmens identisch sein.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-169">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e5b9-170">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6e5b9-170">Relationships</span></span>
<span data-ttu-id="6e5b9-171">Keine</span><span class="sxs-lookup"><span data-stu-id="6e5b9-171">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e5b9-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6e5b9-172">JSON representation</span></span>

<span data-ttu-id="6e5b9-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6e5b9-173">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
