---
title: Ressourcentyp bookingService
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 63eae84249501426c43ad73326cbf005009753be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815442"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="13cf4-104">Ressourcentyp bookingService</span><span class="sxs-lookup"><span data-stu-id="13cf4-104">bookingService resource type</span></span>

 > <span data-ttu-id="13cf4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="13cf4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13cf4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13cf4-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="13cf4-107">Stellt Informationen zu einem bestimmten Dienst stammt von einer [BookingBusiness](bookingbusiness.md), wie der Dienstname, Preis und die Mitarbeiter, die in der Regel ein solcher Dienst bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="13cf4-107">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="13cf4-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="13cf4-108">Methods</span></span>

| <span data-ttu-id="13cf4-109">Methode</span><span class="sxs-lookup"><span data-stu-id="13cf4-109">Method</span></span>           | <span data-ttu-id="13cf4-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="13cf4-110">Return Type</span></span>    |<span data-ttu-id="13cf4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13cf4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13cf4-112">Liste Dienste</span><span class="sxs-lookup"><span data-stu-id="13cf4-112">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="13cf4-113">[BookingService](bookingservice.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="13cf4-113">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="13cf4-114">Rufen Sie eine Liste der **BookingService** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="13cf4-114">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="13cf4-115">Erstellen von bookingService</span><span class="sxs-lookup"><span data-stu-id="13cf4-115">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="13cf4-116">bookingService</span><span class="sxs-lookup"><span data-stu-id="13cf4-116">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="13cf4-117">Erstellen Sie eine **BookingService** für den angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="13cf4-117">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="13cf4-118">Abrufen von bookingService</span><span class="sxs-lookup"><span data-stu-id="13cf4-118">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="13cf4-119">bookingService</span><span class="sxs-lookup"><span data-stu-id="13cf4-119">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="13cf4-120">Rufen Sie die Eigenschaften und die Beziehungen eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="13cf4-120">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="13cf4-121">Update</span><span class="sxs-lookup"><span data-stu-id="13cf4-121">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="13cf4-122">bookingService</span><span class="sxs-lookup"><span data-stu-id="13cf4-122">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="13cf4-123">Aktualisieren eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="13cf4-123">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="13cf4-124">Delete</span><span class="sxs-lookup"><span data-stu-id="13cf4-124">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="13cf4-125">Keine</span><span class="sxs-lookup"><span data-stu-id="13cf4-125">None</span></span> |<span data-ttu-id="13cf4-126">Löschen eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="13cf4-126">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="13cf4-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13cf4-127">Properties</span></span>
| <span data-ttu-id="13cf4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13cf4-128">Property</span></span>     | <span data-ttu-id="13cf4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="13cf4-129">Type</span></span>   |<span data-ttu-id="13cf4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13cf4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13cf4-131">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="13cf4-131">defaultDuration</span></span>|<span data-ttu-id="13cf4-132">Duration</span><span class="sxs-lookup"><span data-stu-id="13cf4-132">Duration</span></span>|<span data-ttu-id="13cf4-133">Die standardmäßige Länge des Diensts, in der Anzahl von Tagen, Stunden, Minuten und Sekunden dargestellt.</span><span class="sxs-lookup"><span data-stu-id="13cf4-133">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="13cf4-134">Beispielsweise P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="13cf4-134">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="13cf4-135">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="13cf4-135">defaultLocation</span></span>|[<span data-ttu-id="13cf4-136">location</span><span class="sxs-lookup"><span data-stu-id="13cf4-136">location</span></span>](location.md)|<span data-ttu-id="13cf4-137">Der physische Standardspeicherort für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="13cf4-137">The default physical location for the service.</span></span>|
|<span data-ttu-id="13cf4-138">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="13cf4-138">defaultPrice</span></span>|<span data-ttu-id="13cf4-139">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="13cf4-139">Double</span></span>|<span data-ttu-id="13cf4-140">Der Standardwert monetäre Preis für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="13cf4-140">The default monetary price for the service.</span></span>|
|<span data-ttu-id="13cf4-141">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="13cf4-141">defaultPriceType</span></span>|<span data-ttu-id="13cf4-142">string</span><span class="sxs-lookup"><span data-stu-id="13cf4-142">string</span></span>|<span data-ttu-id="13cf4-143">Die Standardmethode der Dienst aufgeladen wird.</span><span class="sxs-lookup"><span data-stu-id="13cf4-143">The default way the service is charged.</span></span> <span data-ttu-id="13cf4-144">Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="13cf4-144">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="13cf4-145">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="13cf4-145">defaultReminders</span></span>|<span data-ttu-id="13cf4-146">[BookingReminder](bookingreminder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="13cf4-146">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="13cf4-147">Die Standardeinstellung Festlegen von Erinnerungen für einen Termin dieses Diensts.</span><span class="sxs-lookup"><span data-stu-id="13cf4-147">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="13cf4-148">Der Wert dieser Eigenschaft ist nur bei dieser **BookingService** anhand seiner ID Lesen verfügbar</span><span class="sxs-lookup"><span data-stu-id="13cf4-148">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="13cf4-149">description</span><span class="sxs-lookup"><span data-stu-id="13cf4-149">description</span></span>|<span data-ttu-id="13cf4-150">String</span><span class="sxs-lookup"><span data-stu-id="13cf4-150">String</span></span>|<span data-ttu-id="13cf4-151">Eine Beschreibung für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="13cf4-151">A text description for the service.</span></span>|
|<span data-ttu-id="13cf4-152">displayName</span><span class="sxs-lookup"><span data-stu-id="13cf4-152">displayName</span></span>|<span data-ttu-id="13cf4-153">String</span><span class="sxs-lookup"><span data-stu-id="13cf4-153">String</span></span>|<span data-ttu-id="13cf4-154">Ein Dienstname.</span><span class="sxs-lookup"><span data-stu-id="13cf4-154">A service name.</span></span>|
|<span data-ttu-id="13cf4-155">emailAddress</span><span class="sxs-lookup"><span data-stu-id="13cf4-155">emailAddress</span></span>|<span data-ttu-id="13cf4-156">String</span><span class="sxs-lookup"><span data-stu-id="13cf4-156">String</span></span>|<span data-ttu-id="13cf4-157">Eine e-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="13cf4-157">An email address</span></span>|
|<span data-ttu-id="13cf4-158">id</span><span class="sxs-lookup"><span data-stu-id="13cf4-158">id</span></span>|<span data-ttu-id="13cf4-159">String</span><span class="sxs-lookup"><span data-stu-id="13cf4-159">String</span></span>|<span data-ttu-id="13cf4-160">Die ID des Diensts aus, in einen GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="13cf4-160">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="13cf4-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13cf4-161">Read-only.</span></span>|
|<span data-ttu-id="13cf4-162">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="13cf4-162">isHiddenFromCustomers</span></span>|<span data-ttu-id="13cf4-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="13cf4-163">Boolean</span></span>|<span data-ttu-id="13cf4-164">"True" bedeutet, dass dieser Dienst nicht verfügbar für Kunden für buchen ist.</span><span class="sxs-lookup"><span data-stu-id="13cf4-164">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="13cf4-165">notes</span><span class="sxs-lookup"><span data-stu-id="13cf4-165">notes</span></span>|<span data-ttu-id="13cf4-166">String</span><span class="sxs-lookup"><span data-stu-id="13cf4-166">String</span></span>|<span data-ttu-id="13cf4-167">Weitere Informationen zu diesem Dienst.</span><span class="sxs-lookup"><span data-stu-id="13cf4-167">Additional information about this service.</span></span>|
|<span data-ttu-id="13cf4-168">postBuffer</span><span class="sxs-lookup"><span data-stu-id="13cf4-168">postBuffer</span></span>|<span data-ttu-id="13cf4-169">Duration</span><span class="sxs-lookup"><span data-stu-id="13cf4-169">Duration</span></span>|<span data-ttu-id="13cf4-170">Die Zeit bis zur Puffer nach eines Termins für diesen Dienst beendet, und vor dem nächsten Kunden Termin gebucht werden kann.</span><span class="sxs-lookup"><span data-stu-id="13cf4-170">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="13cf4-171">preBuffer</span><span class="sxs-lookup"><span data-stu-id="13cf4-171">preBuffer</span></span>|<span data-ttu-id="13cf4-172">Duration</span><span class="sxs-lookup"><span data-stu-id="13cf4-172">Duration</span></span>|<span data-ttu-id="13cf4-173">Die Zeit zum Zwischenspeichern, bevor Sie ein Termin für diesen Dienst starten kann.</span><span class="sxs-lookup"><span data-stu-id="13cf4-173">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="13cf4-174">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="13cf4-174">schedulingPolicy</span></span>|[<span data-ttu-id="13cf4-175">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="13cf4-175">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="13cf4-176">Der Satz von Richtlinien, die bestimmen, wie Termine für diesen Dienst erstellt und verwaltet werden soll.</span><span class="sxs-lookup"><span data-stu-id="13cf4-176">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="13cf4-177">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="13cf4-177">staffMemberIds</span></span>|<span data-ttu-id="13cf4-178">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="13cf4-178">String collection</span></span>|<span data-ttu-id="13cf4-179">Stellt die [Mitarbeiter](bookingstaffmember.md) , die diesen Dienst bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="13cf4-179">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="13cf4-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="13cf4-180">Relationships</span></span>
<span data-ttu-id="13cf4-181">Keine</span><span class="sxs-lookup"><span data-stu-id="13cf4-181">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="13cf4-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13cf4-182">JSON representation</span></span>

<span data-ttu-id="13cf4-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13cf4-183">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
