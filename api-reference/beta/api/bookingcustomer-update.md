---
title: Bookingcustomer aktualisieren
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: ccfd7d496f796ea71568a58d48e62ed84c29abc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844345"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="dd012-104">Bookingcustomer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dd012-104">Update bookingcustomer</span></span>

 > <span data-ttu-id="dd012-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd012-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd012-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd012-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="dd012-107">Aktualisieren Sie die Eigenschaften eines [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd012-107">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd012-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd012-108">Permissions</span></span>
<span data-ttu-id="dd012-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd012-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd012-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd012-111">Permission type</span></span>      | <span data-ttu-id="dd012-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd012-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd012-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd012-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dd012-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="dd012-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="dd012-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd012-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd012-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd012-116">Not supported.</span></span>   |
|<span data-ttu-id="dd012-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd012-117">Application</span></span> | <span data-ttu-id="dd012-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd012-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="dd012-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd012-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="dd012-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd012-120">Optional request headers</span></span>
| <span data-ttu-id="dd012-121">Name</span><span class="sxs-lookup"><span data-stu-id="dd012-121">Name</span></span>       | <span data-ttu-id="dd012-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd012-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dd012-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd012-123">Authorization</span></span>  | <span data-ttu-id="dd012-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dd012-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd012-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd012-125">Request body</span></span>
<span data-ttu-id="dd012-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="dd012-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd012-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd012-129">Property</span></span>     | <span data-ttu-id="dd012-130">Typ</span><span class="sxs-lookup"><span data-stu-id="dd012-130">Type</span></span>   |<span data-ttu-id="dd012-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd012-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd012-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dd012-132">displayName</span></span>|<span data-ttu-id="dd012-133">String</span><span class="sxs-lookup"><span data-stu-id="dd012-133">String</span></span>|<span data-ttu-id="dd012-134">Der Name des Kunden.</span><span class="sxs-lookup"><span data-stu-id="dd012-134">The name of the customer.</span></span>|
|<span data-ttu-id="dd012-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dd012-135">emailAddress</span></span>|<span data-ttu-id="dd012-136">String</span><span class="sxs-lookup"><span data-stu-id="dd012-136">String</span></span>|<span data-ttu-id="dd012-137">Die SMTP-Adresse des Kunden.</span><span class="sxs-lookup"><span data-stu-id="dd012-137">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="dd012-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd012-138">Response</span></span>
<span data-ttu-id="dd012-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [BookingCustomer](../resources/bookingcustomer.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dd012-139">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd012-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd012-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd012-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd012-141">Request</span></span>
<span data-ttu-id="dd012-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd012-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="dd012-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd012-143">Response</span></span>
<span data-ttu-id="dd012-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd012-144">The following is an example of the response.</span></span> <span data-ttu-id="dd012-145">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="dd012-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dd012-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd012-146">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
