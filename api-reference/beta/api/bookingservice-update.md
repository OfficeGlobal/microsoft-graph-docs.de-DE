---
title: Bookingservice aktualisieren
description: Aktualisieren Sie die Eigenschaften eines BookingService-Objekts in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519717"
---
# <a name="update-bookingservice"></a><span data-ttu-id="c2ed9-103">Bookingservice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c2ed9-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ed9-104">Aktualisieren Sie die Eigenschaften eines [BookingService](../resources/bookingservice.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="c2ed9-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="c2ed9-105">Es folgen einige Beispiele, die Sie für einen Dienst anpassen können:</span><span class="sxs-lookup"><span data-stu-id="c2ed9-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="c2ed9-106">Kurs</span><span class="sxs-lookup"><span data-stu-id="c2ed9-106">Price</span></span>
- <span data-ttu-id="c2ed9-107">Typische Länge eines Termins</span><span class="sxs-lookup"><span data-stu-id="c2ed9-107">Typical length of an appointment</span></span>
- <span data-ttu-id="c2ed9-108">Erinnerungen</span><span class="sxs-lookup"><span data-stu-id="c2ed9-108">Reminders</span></span>
- <span data-ttu-id="c2ed9-109">Jedes Mal, wenn Puffer, richten Sie vor oder nach der Service abschließen</span><span class="sxs-lookup"><span data-stu-id="c2ed9-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="c2ed9-110">[Planen von Richtlinien](../resources/bookingschedulingpolicy.md) Parameter wie minimale Hinweis zum Buch oder Abbrechen, und ob Kunden bestimmte Mitarbeiter für einen Termin auswählen können.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2ed9-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c2ed9-111">Permissions</span></span>
<span data-ttu-id="c2ed9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2ed9-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2ed9-114">Permission type</span></span>      | <span data-ttu-id="c2ed9-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2ed9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ed9-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2ed9-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="c2ed9-117">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c2ed9-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c2ed9-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2ed9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ed9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2ed9-119">Not supported.</span></span>   |
|<span data-ttu-id="c2ed9-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-120">Application</span></span> | <span data-ttu-id="c2ed9-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2ed9-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c2ed9-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c2ed9-123">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2ed9-123">Optional request headers</span></span>
| <span data-ttu-id="c2ed9-124">Name</span><span class="sxs-lookup"><span data-stu-id="c2ed9-124">Name</span></span>       | <span data-ttu-id="c2ed9-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c2ed9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2ed9-126">Authorization</span></span>  | <span data-ttu-id="c2ed9-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c2ed9-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2ed9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2ed9-128">Request body</span></span>
<span data-ttu-id="c2ed9-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2ed9-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2ed9-132">Property</span></span>     | <span data-ttu-id="c2ed9-133">Typ</span><span class="sxs-lookup"><span data-stu-id="c2ed9-133">Type</span></span>   |<span data-ttu-id="c2ed9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2ed9-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="c2ed9-135">defaultDuration</span></span>|<span data-ttu-id="c2ed9-136">Dauer</span><span class="sxs-lookup"><span data-stu-id="c2ed9-136">Duration</span></span>|<span data-ttu-id="c2ed9-137">Die standardmäßige Länge des Diensts, in der Anzahl von Tagen, Stunden, Minuten und Sekunden dargestellt.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="c2ed9-138">Beispielsweise P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="c2ed9-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="c2ed9-139">defaultLocation</span></span>|[<span data-ttu-id="c2ed9-140">location</span><span class="sxs-lookup"><span data-stu-id="c2ed9-140">location</span></span>](../resources/location.md)|<span data-ttu-id="c2ed9-141">Der physische Standardspeicherort für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="c2ed9-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="c2ed9-142">defaultPrice</span></span>|<span data-ttu-id="c2ed9-143">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="c2ed9-143">Double</span></span>|<span data-ttu-id="c2ed9-144">Der Standardwert monetäre Preis für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="c2ed9-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="c2ed9-145">defaultPriceType</span></span>|<span data-ttu-id="c2ed9-146">string</span><span class="sxs-lookup"><span data-stu-id="c2ed9-146">string</span></span>|<span data-ttu-id="c2ed9-147">Die Standardmethode der Dienst aufgeladen wird.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-147">The default way the service is charged.</span></span> <span data-ttu-id="c2ed9-148">Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="c2ed9-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="c2ed9-149">defaultReminders</span></span>|<span data-ttu-id="c2ed9-150">[BookingReminder](../resources/bookingreminder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="c2ed9-151">Die Standardeinstellung Festlegen von Erinnerungen für einen Termin dieses Diensts.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="c2ed9-152">Der Wert dieser Eigenschaft ist nur bei dieser **BookingService** anhand seiner ID Lesen verfügbar</span><span class="sxs-lookup"><span data-stu-id="c2ed9-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="c2ed9-153">description</span><span class="sxs-lookup"><span data-stu-id="c2ed9-153">description</span></span>|<span data-ttu-id="c2ed9-154">String</span><span class="sxs-lookup"><span data-stu-id="c2ed9-154">String</span></span>|<span data-ttu-id="c2ed9-155">Eine Beschreibung für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-155">A text description for the service.</span></span>|
|<span data-ttu-id="c2ed9-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c2ed9-156">displayName</span></span>|<span data-ttu-id="c2ed9-157">String</span><span class="sxs-lookup"><span data-stu-id="c2ed9-157">String</span></span>|<span data-ttu-id="c2ed9-158">Ein Dienstname.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-158">A service name.</span></span>|
|<span data-ttu-id="c2ed9-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c2ed9-159">emailAddress</span></span>|<span data-ttu-id="c2ed9-160">String</span><span class="sxs-lookup"><span data-stu-id="c2ed9-160">String</span></span>|<span data-ttu-id="c2ed9-161">Eine E-Mail-Adresse:  </span><span class="sxs-lookup"><span data-stu-id="c2ed9-161">An email address</span></span>|
|<span data-ttu-id="c2ed9-162">id</span><span class="sxs-lookup"><span data-stu-id="c2ed9-162">id</span></span>|<span data-ttu-id="c2ed9-163">String</span><span class="sxs-lookup"><span data-stu-id="c2ed9-163">String</span></span>| <span data-ttu-id="c2ed9-164">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-164">Read-only.</span></span>|
|<span data-ttu-id="c2ed9-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="c2ed9-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="c2ed9-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c2ed9-166">Boolean</span></span>|<span data-ttu-id="c2ed9-167">"True" bedeutet, dass dieser Dienst nicht verfügbar für Kunden für buchen ist.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="c2ed9-168">notes</span><span class="sxs-lookup"><span data-stu-id="c2ed9-168">notes</span></span>|<span data-ttu-id="c2ed9-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ed9-169">String</span></span>|<span data-ttu-id="c2ed9-170">Weitere Informationen zu diesem Dienst.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-170">Additional information about this service.</span></span>|
|<span data-ttu-id="c2ed9-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="c2ed9-171">postBuffer</span></span>|<span data-ttu-id="c2ed9-172">Dauer</span><span class="sxs-lookup"><span data-stu-id="c2ed9-172">Duration</span></span>|<span data-ttu-id="c2ed9-173">Die Zeit bis zur Puffer nach eines Termins für diesen Dienst beendet, und vor dem nächsten Kunden Termin gebucht werden kann.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="c2ed9-174">preBuffer</span><span class="sxs-lookup"><span data-stu-id="c2ed9-174">preBuffer</span></span>|<span data-ttu-id="c2ed9-175">Dauer</span><span class="sxs-lookup"><span data-stu-id="c2ed9-175">Duration</span></span>|<span data-ttu-id="c2ed9-176">Die Zeit zum Zwischenspeichern, bevor Sie ein Termin für diesen Dienst starten kann.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="c2ed9-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c2ed9-177">schedulingPolicy</span></span>|[<span data-ttu-id="c2ed9-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c2ed9-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="c2ed9-179">Der Satz von Richtlinien, die bestimmen, wie Termine für diesen Dienst erstellt und verwaltet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="c2ed9-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="c2ed9-180">staffMemberIds</span></span>|<span data-ttu-id="c2ed9-181">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-181">String collection</span></span>|<span data-ttu-id="c2ed9-182">Stellt die [Mitarbeiter](../resources/bookingstaffmember.md) , die diesen Dienst bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="c2ed9-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2ed9-183">Response</span></span>
<span data-ttu-id="c2ed9-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2ed9-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2ed9-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2ed9-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2ed9-187">Request</span></span>
<span data-ttu-id="c2ed9-188">Im folgende Beispiel wird die Dauer des angegebenen Dienstes aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-188">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c2ed9-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2ed9-189">Response</span></span>
<span data-ttu-id="c2ed9-190">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c2ed9-190">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
