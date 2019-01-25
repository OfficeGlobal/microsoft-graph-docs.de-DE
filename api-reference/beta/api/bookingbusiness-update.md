---
title: Bookingbusiness aktualisieren
description: Aktualisieren Sie die Eigenschaften eines BookingBusiness-Objekts.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dba24dafef030ae53fc83fb06d1cc7b99ed71e81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528802"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="114aa-103">Bookingbusiness aktualisieren</span><span class="sxs-lookup"><span data-stu-id="114aa-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="114aa-104">Aktualisieren Sie die Eigenschaften eines [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="114aa-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="114aa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="114aa-105">Permissions</span></span>
<span data-ttu-id="114aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="114aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="114aa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="114aa-108">Permission type</span></span>      | <span data-ttu-id="114aa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="114aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="114aa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="114aa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="114aa-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="114aa-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="114aa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="114aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="114aa-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="114aa-113">Not supported.</span></span>   |
|<span data-ttu-id="114aa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="114aa-114">Application</span></span> | <span data-ttu-id="114aa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="114aa-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="114aa-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="114aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="114aa-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="114aa-117">Optional request headers</span></span>
| <span data-ttu-id="114aa-118">Name</span><span class="sxs-lookup"><span data-stu-id="114aa-118">Name</span></span>       | <span data-ttu-id="114aa-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="114aa-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="114aa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="114aa-120">Authorization</span></span>  | <span data-ttu-id="114aa-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="114aa-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="114aa-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="114aa-122">Request body</span></span>
<span data-ttu-id="114aa-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="114aa-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="114aa-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="114aa-126">Property</span></span>     | <span data-ttu-id="114aa-127">Typ</span><span class="sxs-lookup"><span data-stu-id="114aa-127">Type</span></span>   |<span data-ttu-id="114aa-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="114aa-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="114aa-129">address</span><span class="sxs-lookup"><span data-stu-id="114aa-129">address</span></span>|[<span data-ttu-id="114aa-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="114aa-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="114aa-131">Die Straße des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="114aa-131">The street address of the business.</span></span>|
|<span data-ttu-id="114aa-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="114aa-132">businessHours</span></span>|<span data-ttu-id="114aa-133">[BookingWorkHours](../resources/bookingworkhours.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="114aa-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="114aa-134">Die Betriebszeiten für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="114aa-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="114aa-135">businessType</span><span class="sxs-lookup"><span data-stu-id="114aa-135">businessType</span></span>|<span data-ttu-id="114aa-136">String</span><span class="sxs-lookup"><span data-stu-id="114aa-136">String</span></span>|<span data-ttu-id="114aa-137">Der Typ des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="114aa-137">The type of business.</span></span>|
|<span data-ttu-id="114aa-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="114aa-138">defaultCurrencyIso</span></span>|<span data-ttu-id="114aa-139">String</span><span class="sxs-lookup"><span data-stu-id="114aa-139">String</span></span>|<span data-ttu-id="114aa-140">Der Code für die Währung, die das Unternehmen in für Microsoft Bookings ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="114aa-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="114aa-141">displayName</span><span class="sxs-lookup"><span data-stu-id="114aa-141">displayName</span></span>|<span data-ttu-id="114aa-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="114aa-142">String</span></span>|<span data-ttu-id="114aa-143">Ein Name für das Unternehmen, das mit Kunden-Schnittstellen.</span><span class="sxs-lookup"><span data-stu-id="114aa-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="114aa-144">E-Mail</span><span class="sxs-lookup"><span data-stu-id="114aa-144">email</span></span>|<span data-ttu-id="114aa-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="114aa-145">String</span></span>|<span data-ttu-id="114aa-146">Die e-Mail-Adresse für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="114aa-146">The email address for the business.</span></span>|
|<span data-ttu-id="114aa-147">phone</span><span class="sxs-lookup"><span data-stu-id="114aa-147">phone</span></span>|<span data-ttu-id="114aa-148">String</span><span class="sxs-lookup"><span data-stu-id="114aa-148">String</span></span>|<span data-ttu-id="114aa-149">Die Telefonnummer für das Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="114aa-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="114aa-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="114aa-150">schedulingPolicy</span></span>|[<span data-ttu-id="114aa-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="114aa-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="114aa-152">Gibt an, wie die Buchungen für dieses Unternehmen erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="114aa-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="114aa-153">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="114aa-153">webSiteUrl</span></span>|<span data-ttu-id="114aa-154">String</span><span class="sxs-lookup"><span data-stu-id="114aa-154">String</span></span>|<span data-ttu-id="114aa-155">Die URL der Website für die Business.</span><span class="sxs-lookup"><span data-stu-id="114aa-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="114aa-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="114aa-156">Response</span></span>
<span data-ttu-id="114aa-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="114aa-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="114aa-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="114aa-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="114aa-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="114aa-160">Request</span></span>
<span data-ttu-id="114aa-161">Das folgende Beispiel aktualisiert die geschäftliche e-Mail-Adresse und Planen von Richtlinien, ändern Sie das Zeitintervall für Business Standard buchen in eine Stunde und bis zu 30 Tage buchungs-wechseln.</span><span class="sxs-lookup"><span data-stu-id="114aa-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="114aa-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="114aa-162">Response</span></span>
<span data-ttu-id="114aa-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="114aa-163">The following is an example of the response.</span></span> <span data-ttu-id="114aa-164">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="114aa-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="114aa-165">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="114aa-165">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
