---
title: Bookingservice aktualisieren
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6830ebc8fc101c4c9ce60f6157ed6bfdab82748c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937040"
---
# <a name="update-bookingservice"></a><span data-ttu-id="cd995-104">Bookingservice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cd995-104">Update bookingservice</span></span>

 > <span data-ttu-id="cd995-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cd995-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd995-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd995-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="cd995-107">Aktualisieren Sie die Eigenschaften eines [BookingService](../resources/bookingservice.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="cd995-107">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="cd995-108">Es folgen einige Beispiele, die Sie für einen Dienst anpassen können:</span><span class="sxs-lookup"><span data-stu-id="cd995-108">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="cd995-109">Kurs</span><span class="sxs-lookup"><span data-stu-id="cd995-109">Price</span></span>
- <span data-ttu-id="cd995-110">Typische Länge eines Termins</span><span class="sxs-lookup"><span data-stu-id="cd995-110">Typical length of an appointment</span></span>
- <span data-ttu-id="cd995-111">Erinnerungen</span><span class="sxs-lookup"><span data-stu-id="cd995-111">Reminders</span></span>
- <span data-ttu-id="cd995-112">Jedes Mal, wenn Puffer, richten Sie vor oder nach der Service abschließen</span><span class="sxs-lookup"><span data-stu-id="cd995-112">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="cd995-113">[Planen von Richtlinien](../resources/bookingschedulingpolicy.md) Parameter wie minimale Hinweis zum Buch oder Abbrechen, und ob Kunden bestimmte Mitarbeiter für einen Termin auswählen können.</span><span class="sxs-lookup"><span data-stu-id="cd995-113">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd995-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd995-114">Permissions</span></span>
<span data-ttu-id="cd995-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd995-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd995-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd995-117">Permission type</span></span>      | <span data-ttu-id="cd995-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd995-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd995-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd995-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="cd995-120">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="cd995-120">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cd995-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd995-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd995-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd995-122">Not supported.</span></span>   |
|<span data-ttu-id="cd995-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd995-123">Application</span></span> | <span data-ttu-id="cd995-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd995-124">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cd995-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd995-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cd995-126">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd995-126">Optional request headers</span></span>
| <span data-ttu-id="cd995-127">Name</span><span class="sxs-lookup"><span data-stu-id="cd995-127">Name</span></span>       | <span data-ttu-id="cd995-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd995-128">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cd995-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd995-129">Authorization</span></span>  | <span data-ttu-id="cd995-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cd995-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd995-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd995-131">Request body</span></span>
<span data-ttu-id="cd995-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="cd995-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd995-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd995-135">Property</span></span>     | <span data-ttu-id="cd995-136">Typ</span><span class="sxs-lookup"><span data-stu-id="cd995-136">Type</span></span>   |<span data-ttu-id="cd995-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd995-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd995-138">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="cd995-138">defaultDuration</span></span>|<span data-ttu-id="cd995-139">Duration</span><span class="sxs-lookup"><span data-stu-id="cd995-139">Duration</span></span>|<span data-ttu-id="cd995-140">Die standardmäßige Länge des Diensts, in der Anzahl von Tagen, Stunden, Minuten und Sekunden dargestellt.</span><span class="sxs-lookup"><span data-stu-id="cd995-140">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="cd995-141">Beispielsweise P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="cd995-141">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="cd995-142">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="cd995-142">defaultLocation</span></span>|[<span data-ttu-id="cd995-143">location</span><span class="sxs-lookup"><span data-stu-id="cd995-143">location</span></span>](../resources/location.md)|<span data-ttu-id="cd995-144">Der physische Standardspeicherort für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="cd995-144">The default physical location for the service.</span></span>|
|<span data-ttu-id="cd995-145">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="cd995-145">defaultPrice</span></span>|<span data-ttu-id="cd995-146">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="cd995-146">Double</span></span>|<span data-ttu-id="cd995-147">Der Standardwert monetäre Preis für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="cd995-147">The default monetary price for the service.</span></span>|
|<span data-ttu-id="cd995-148">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="cd995-148">defaultPriceType</span></span>|<span data-ttu-id="cd995-149">string</span><span class="sxs-lookup"><span data-stu-id="cd995-149">string</span></span>|<span data-ttu-id="cd995-150">Die Standardmethode der Dienst aufgeladen wird.</span><span class="sxs-lookup"><span data-stu-id="cd995-150">The default way the service is charged.</span></span> <span data-ttu-id="cd995-151">Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="cd995-151">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="cd995-152">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="cd995-152">defaultReminders</span></span>|<span data-ttu-id="cd995-153">[BookingReminder](../resources/bookingreminder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="cd995-153">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="cd995-154">Die Standardeinstellung Festlegen von Erinnerungen für einen Termin dieses Diensts.</span><span class="sxs-lookup"><span data-stu-id="cd995-154">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="cd995-155">Der Wert dieser Eigenschaft ist nur bei dieser **BookingService** anhand seiner ID Lesen verfügbar</span><span class="sxs-lookup"><span data-stu-id="cd995-155">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="cd995-156">description</span><span class="sxs-lookup"><span data-stu-id="cd995-156">description</span></span>|<span data-ttu-id="cd995-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd995-157">String</span></span>|<span data-ttu-id="cd995-158">Eine Beschreibung für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="cd995-158">A text description for the service.</span></span>|
|<span data-ttu-id="cd995-159">displayName</span><span class="sxs-lookup"><span data-stu-id="cd995-159">displayName</span></span>|<span data-ttu-id="cd995-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd995-160">String</span></span>|<span data-ttu-id="cd995-161">Ein Dienstname.</span><span class="sxs-lookup"><span data-stu-id="cd995-161">A service name.</span></span>|
|<span data-ttu-id="cd995-162">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cd995-162">emailAddress</span></span>|<span data-ttu-id="cd995-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd995-163">String</span></span>|<span data-ttu-id="cd995-164">Eine e-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="cd995-164">An email address</span></span>|
|<span data-ttu-id="cd995-165">id</span><span class="sxs-lookup"><span data-stu-id="cd995-165">id</span></span>|<span data-ttu-id="cd995-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd995-166">String</span></span>| <span data-ttu-id="cd995-167">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cd995-167">Read-only.</span></span>|
|<span data-ttu-id="cd995-168">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="cd995-168">isHiddenFromCustomers</span></span>|<span data-ttu-id="cd995-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cd995-169">Boolean</span></span>|<span data-ttu-id="cd995-170">"True" bedeutet, dass dieser Dienst nicht verfügbar für Kunden für buchen ist.</span><span class="sxs-lookup"><span data-stu-id="cd995-170">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="cd995-171">notes</span><span class="sxs-lookup"><span data-stu-id="cd995-171">notes</span></span>|<span data-ttu-id="cd995-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd995-172">String</span></span>|<span data-ttu-id="cd995-173">Weitere Informationen zu diesem Dienst.</span><span class="sxs-lookup"><span data-stu-id="cd995-173">Additional information about this service.</span></span>|
|<span data-ttu-id="cd995-174">postBuffer</span><span class="sxs-lookup"><span data-stu-id="cd995-174">postBuffer</span></span>|<span data-ttu-id="cd995-175">Duration</span><span class="sxs-lookup"><span data-stu-id="cd995-175">Duration</span></span>|<span data-ttu-id="cd995-176">Die Zeit bis zur Puffer nach eines Termins für diesen Dienst beendet, und vor dem nächsten Kunden Termin gebucht werden kann.</span><span class="sxs-lookup"><span data-stu-id="cd995-176">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="cd995-177">preBuffer</span><span class="sxs-lookup"><span data-stu-id="cd995-177">preBuffer</span></span>|<span data-ttu-id="cd995-178">Duration</span><span class="sxs-lookup"><span data-stu-id="cd995-178">Duration</span></span>|<span data-ttu-id="cd995-179">Die Zeit zum Zwischenspeichern, bevor Sie ein Termin für diesen Dienst starten kann.</span><span class="sxs-lookup"><span data-stu-id="cd995-179">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="cd995-180">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="cd995-180">schedulingPolicy</span></span>|[<span data-ttu-id="cd995-181">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="cd995-181">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="cd995-182">Der Satz von Richtlinien, die bestimmen, wie Termine für diesen Dienst erstellt und verwaltet werden soll.</span><span class="sxs-lookup"><span data-stu-id="cd995-182">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="cd995-183">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="cd995-183">staffMemberIds</span></span>|<span data-ttu-id="cd995-184">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="cd995-184">String collection</span></span>|<span data-ttu-id="cd995-185">Stellt die [Mitarbeiter](../resources/bookingstaffmember.md) , die diesen Dienst bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="cd995-185">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="cd995-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd995-186">Response</span></span>
<span data-ttu-id="cd995-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd995-p108">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd995-189">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd995-189">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd995-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd995-190">Request</span></span>
<span data-ttu-id="cd995-191">Im folgende Beispiel wird die Dauer des angegebenen Dienstes aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cd995-191">The following example updates the duration of the specified service.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a><span data-ttu-id="cd995-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd995-192">Response</span></span>
<span data-ttu-id="cd995-193">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd995-193">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
