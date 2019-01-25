---
title: Ressourcentyp bookingService
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519885"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="3d302-104">Ressourcentyp bookingService</span><span class="sxs-lookup"><span data-stu-id="3d302-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3d302-105">Stellt Informationen zu einem bestimmten Dienst stammt von einer [BookingBusiness](bookingbusiness.md), wie der Dienstname, Preis und die Mitarbeiter, die in der Regel ein solcher Dienst bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="3d302-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="3d302-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="3d302-106">Methods</span></span>

| <span data-ttu-id="3d302-107">Methode</span><span class="sxs-lookup"><span data-stu-id="3d302-107">Method</span></span>           | <span data-ttu-id="3d302-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3d302-108">Return Type</span></span>    |<span data-ttu-id="3d302-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d302-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d302-110">Liste Dienste</span><span class="sxs-lookup"><span data-stu-id="3d302-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="3d302-111">[BookingService](bookingservice.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3d302-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="3d302-112">Rufen Sie eine Liste der **BookingService** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3d302-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="3d302-113">Erstellen von bookingService</span><span class="sxs-lookup"><span data-stu-id="3d302-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="3d302-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="3d302-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="3d302-115">Erstellen Sie eine **BookingService** für den angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3d302-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="3d302-116">Abrufen von bookingService</span><span class="sxs-lookup"><span data-stu-id="3d302-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="3d302-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="3d302-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="3d302-118">Rufen Sie die Eigenschaften und die Beziehungen eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3d302-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="3d302-119">Update</span><span class="sxs-lookup"><span data-stu-id="3d302-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="3d302-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="3d302-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="3d302-121">Aktualisieren eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3d302-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="3d302-122">Delete</span><span class="sxs-lookup"><span data-stu-id="3d302-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="3d302-123">Keine</span><span class="sxs-lookup"><span data-stu-id="3d302-123">None</span></span> |<span data-ttu-id="3d302-124">Löschen eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3d302-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="3d302-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d302-125">Properties</span></span>
| <span data-ttu-id="3d302-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d302-126">Property</span></span>     | <span data-ttu-id="3d302-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3d302-127">Type</span></span>   |<span data-ttu-id="3d302-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d302-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d302-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="3d302-129">defaultDuration</span></span>|<span data-ttu-id="3d302-130">Dauer</span><span class="sxs-lookup"><span data-stu-id="3d302-130">Duration</span></span>|<span data-ttu-id="3d302-131">Die standardmäßige Länge des Diensts, in der Anzahl von Tagen, Stunden, Minuten und Sekunden dargestellt.</span><span class="sxs-lookup"><span data-stu-id="3d302-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="3d302-132">Beispielsweise P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="3d302-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="3d302-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="3d302-133">defaultLocation</span></span>|[<span data-ttu-id="3d302-134">location</span><span class="sxs-lookup"><span data-stu-id="3d302-134">location</span></span>](location.md)|<span data-ttu-id="3d302-135">Der physische Standardspeicherort für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="3d302-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="3d302-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="3d302-136">defaultPrice</span></span>|<span data-ttu-id="3d302-137">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="3d302-137">Double</span></span>|<span data-ttu-id="3d302-138">Der Standardwert monetäre Preis für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="3d302-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="3d302-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="3d302-139">defaultPriceType</span></span>|<span data-ttu-id="3d302-140">string</span><span class="sxs-lookup"><span data-stu-id="3d302-140">string</span></span>|<span data-ttu-id="3d302-141">Die Standardmethode der Dienst aufgeladen wird.</span><span class="sxs-lookup"><span data-stu-id="3d302-141">The default way the service is charged.</span></span> <span data-ttu-id="3d302-142">Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3d302-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="3d302-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="3d302-143">defaultReminders</span></span>|<span data-ttu-id="3d302-144">[BookingReminder](bookingreminder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3d302-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="3d302-145">Die Standardeinstellung Festlegen von Erinnerungen für einen Termin dieses Diensts.</span><span class="sxs-lookup"><span data-stu-id="3d302-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="3d302-146">Der Wert dieser Eigenschaft ist nur bei dieser **BookingService** anhand seiner ID Lesen verfügbar</span><span class="sxs-lookup"><span data-stu-id="3d302-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="3d302-147">description</span><span class="sxs-lookup"><span data-stu-id="3d302-147">description</span></span>|<span data-ttu-id="3d302-148">String</span><span class="sxs-lookup"><span data-stu-id="3d302-148">String</span></span>|<span data-ttu-id="3d302-149">Eine Beschreibung für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="3d302-149">A text description for the service.</span></span>|
|<span data-ttu-id="3d302-150">displayName</span><span class="sxs-lookup"><span data-stu-id="3d302-150">displayName</span></span>|<span data-ttu-id="3d302-151">String</span><span class="sxs-lookup"><span data-stu-id="3d302-151">String</span></span>|<span data-ttu-id="3d302-152">Ein Dienstname.</span><span class="sxs-lookup"><span data-stu-id="3d302-152">A service name.</span></span>|
|<span data-ttu-id="3d302-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3d302-153">emailAddress</span></span>|<span data-ttu-id="3d302-154">String</span><span class="sxs-lookup"><span data-stu-id="3d302-154">String</span></span>|<span data-ttu-id="3d302-155">Eine E-Mail-Adresse:  </span><span class="sxs-lookup"><span data-stu-id="3d302-155">An email address</span></span>|
|<span data-ttu-id="3d302-156">id</span><span class="sxs-lookup"><span data-stu-id="3d302-156">id</span></span>|<span data-ttu-id="3d302-157">string</span><span class="sxs-lookup"><span data-stu-id="3d302-157">String</span></span>|<span data-ttu-id="3d302-158">Die ID des Diensts aus, in einen GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="3d302-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="3d302-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3d302-159">Read-only.</span></span>|
|<span data-ttu-id="3d302-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="3d302-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="3d302-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3d302-161">Boolean</span></span>|<span data-ttu-id="3d302-162">"True" bedeutet, dass dieser Dienst nicht verfügbar für Kunden für buchen ist.</span><span class="sxs-lookup"><span data-stu-id="3d302-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="3d302-163">notes</span><span class="sxs-lookup"><span data-stu-id="3d302-163">notes</span></span>|<span data-ttu-id="3d302-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d302-164">String</span></span>|<span data-ttu-id="3d302-165">Weitere Informationen zu diesem Dienst.</span><span class="sxs-lookup"><span data-stu-id="3d302-165">Additional information about this service.</span></span>|
|<span data-ttu-id="3d302-166">postBuffer</span><span class="sxs-lookup"><span data-stu-id="3d302-166">postBuffer</span></span>|<span data-ttu-id="3d302-167">Dauer</span><span class="sxs-lookup"><span data-stu-id="3d302-167">Duration</span></span>|<span data-ttu-id="3d302-168">Die Zeit bis zur Puffer nach eines Termins für diesen Dienst beendet, und vor dem nächsten Kunden Termin gebucht werden kann.</span><span class="sxs-lookup"><span data-stu-id="3d302-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="3d302-169">preBuffer</span><span class="sxs-lookup"><span data-stu-id="3d302-169">preBuffer</span></span>|<span data-ttu-id="3d302-170">Dauer</span><span class="sxs-lookup"><span data-stu-id="3d302-170">Duration</span></span>|<span data-ttu-id="3d302-171">Die Zeit zum Zwischenspeichern, bevor Sie ein Termin für diesen Dienst starten kann.</span><span class="sxs-lookup"><span data-stu-id="3d302-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="3d302-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="3d302-172">schedulingPolicy</span></span>|[<span data-ttu-id="3d302-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="3d302-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="3d302-174">Der Satz von Richtlinien, die bestimmen, wie Termine für diesen Dienst erstellt und verwaltet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3d302-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="3d302-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="3d302-175">staffMemberIds</span></span>|<span data-ttu-id="3d302-176">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3d302-176">String collection</span></span>|<span data-ttu-id="3d302-177">Stellt die [Mitarbeiter](bookingstaffmember.md) , die diesen Dienst bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="3d302-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3d302-178">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3d302-178">Relationships</span></span>
<span data-ttu-id="3d302-179">Keine</span><span class="sxs-lookup"><span data-stu-id="3d302-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3d302-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d302-180">JSON representation</span></span>

<span data-ttu-id="3d302-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d302-181">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
