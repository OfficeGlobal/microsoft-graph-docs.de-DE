---
title: Bookingbusiness aktualisieren
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3f20d466614e35cce701999fabfb631e081a02ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991336"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="be23c-104">Bookingbusiness aktualisieren</span><span class="sxs-lookup"><span data-stu-id="be23c-104">Update bookingbusiness</span></span>

 > <span data-ttu-id="be23c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be23c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be23c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be23c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="be23c-107">Aktualisieren Sie die Eigenschaften eines [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="be23c-107">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be23c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be23c-108">Permissions</span></span>
<span data-ttu-id="be23c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be23c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be23c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be23c-111">Permission type</span></span>      | <span data-ttu-id="be23c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be23c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be23c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be23c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="be23c-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="be23c-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="be23c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be23c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be23c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be23c-116">Not supported.</span></span>   |
|<span data-ttu-id="be23c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be23c-117">Application</span></span> | <span data-ttu-id="be23c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be23c-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="be23c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be23c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="be23c-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be23c-120">Optional request headers</span></span>
| <span data-ttu-id="be23c-121">Name</span><span class="sxs-lookup"><span data-stu-id="be23c-121">Name</span></span>       | <span data-ttu-id="be23c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be23c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="be23c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be23c-123">Authorization</span></span>  | <span data-ttu-id="be23c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="be23c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="be23c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be23c-125">Request body</span></span>
<span data-ttu-id="be23c-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="be23c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="be23c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be23c-129">Property</span></span>     | <span data-ttu-id="be23c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="be23c-130">Type</span></span>   |<span data-ttu-id="be23c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be23c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be23c-132">address</span><span class="sxs-lookup"><span data-stu-id="be23c-132">address</span></span>|[<span data-ttu-id="be23c-133">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="be23c-133">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="be23c-134">Die Straße des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="be23c-134">The street address of the business.</span></span>|
|<span data-ttu-id="be23c-135">businessHours</span><span class="sxs-lookup"><span data-stu-id="be23c-135">businessHours</span></span>|<span data-ttu-id="be23c-136">[BookingWorkHours](../resources/bookingworkhours.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="be23c-136">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="be23c-137">Die Betriebszeiten für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="be23c-137">The hours of operation for the business.</span></span>|
|<span data-ttu-id="be23c-138">businessType</span><span class="sxs-lookup"><span data-stu-id="be23c-138">businessType</span></span>|<span data-ttu-id="be23c-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be23c-139">String</span></span>|<span data-ttu-id="be23c-140">Der Typ des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="be23c-140">The type of business.</span></span>|
|<span data-ttu-id="be23c-141">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="be23c-141">defaultCurrencyIso</span></span>|<span data-ttu-id="be23c-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be23c-142">String</span></span>|<span data-ttu-id="be23c-143">Der Code für die Währung, die das Unternehmen in für Microsoft Bookings ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="be23c-143">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="be23c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="be23c-144">displayName</span></span>|<span data-ttu-id="be23c-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be23c-145">String</span></span>|<span data-ttu-id="be23c-146">Ein Name für das Unternehmen, das mit Kunden-Schnittstellen.</span><span class="sxs-lookup"><span data-stu-id="be23c-146">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="be23c-147">E-Mail</span><span class="sxs-lookup"><span data-stu-id="be23c-147">email</span></span>|<span data-ttu-id="be23c-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be23c-148">String</span></span>|<span data-ttu-id="be23c-149">Die e-Mail-Adresse für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="be23c-149">The email address for the business.</span></span>|
|<span data-ttu-id="be23c-150">phone</span><span class="sxs-lookup"><span data-stu-id="be23c-150">phone</span></span>|<span data-ttu-id="be23c-151">String</span><span class="sxs-lookup"><span data-stu-id="be23c-151">String</span></span>|<span data-ttu-id="be23c-152">Die Telefonnummer für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="be23c-152">The telephone number for the business.</span></span>|
|<span data-ttu-id="be23c-153">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="be23c-153">schedulingPolicy</span></span>|[<span data-ttu-id="be23c-154">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="be23c-154">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="be23c-155">Gibt an, wie die Buchungen für dieses Unternehmen erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="be23c-155">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="be23c-156">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="be23c-156">webSiteUrl</span></span>|<span data-ttu-id="be23c-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be23c-157">String</span></span>|<span data-ttu-id="be23c-158">Die URL der Website für die Business.</span><span class="sxs-lookup"><span data-stu-id="be23c-158">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="be23c-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="be23c-159">Response</span></span>
<span data-ttu-id="be23c-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be23c-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be23c-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be23c-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be23c-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be23c-163">Request</span></span>
<span data-ttu-id="be23c-164">Das folgende Beispiel aktualisiert die geschäftliche e-Mail-Adresse und Planen von Richtlinien, ändern Sie das Zeitintervall für Business Standard buchen in eine Stunde und bis zu 30 Tage buchungs-wechseln.</span><span class="sxs-lookup"><span data-stu-id="be23c-164">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="be23c-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="be23c-165">Response</span></span>
<span data-ttu-id="be23c-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be23c-166">The following is an example of the response.</span></span> <span data-ttu-id="be23c-167">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="be23c-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="be23c-168">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be23c-168">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
