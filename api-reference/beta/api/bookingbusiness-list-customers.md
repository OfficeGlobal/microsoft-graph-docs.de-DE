---
title: Liste von Kunden
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: a46e8dcc39b69e8391829c176eb01d075d23fccf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060026"
---
# <a name="list-customers"></a><span data-ttu-id="0e1b9-104">Liste von Kunden</span><span class="sxs-lookup"><span data-stu-id="0e1b9-104">List customers</span></span>

 > <span data-ttu-id="0e1b9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e1b9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="0e1b9-107">Abrufen einer Liste von [BookingCustomer](../resources/bookingcustomer.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-107">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e1b9-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e1b9-108">Permissions</span></span>
<span data-ttu-id="0e1b9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e1b9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e1b9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e1b9-111">Permission type</span></span>      | <span data-ttu-id="0e1b9-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e1b9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e1b9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e1b9-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0e1b9-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0e1b9-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0e1b9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e1b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e1b9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e1b9-116">Not supported.</span></span>   |
|<span data-ttu-id="0e1b9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e1b9-117">Application</span></span> | <span data-ttu-id="0e1b9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e1b9-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="0e1b9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e1b9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e1b9-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0e1b9-120">Optional query parameters</span></span>
<span data-ttu-id="0e1b9-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e1b9-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e1b9-122">Request headers</span></span>
| <span data-ttu-id="0e1b9-123">Name</span><span class="sxs-lookup"><span data-stu-id="0e1b9-123">Name</span></span>      |<span data-ttu-id="0e1b9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e1b9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e1b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e1b9-125">Authorization</span></span>  | <span data-ttu-id="0e1b9-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0e1b9-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e1b9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e1b9-127">Request body</span></span>
<span data-ttu-id="0e1b9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0e1b9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e1b9-129">Response</span></span>
<span data-ttu-id="0e1b9-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="0e1b9-130">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e1b9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e1b9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e1b9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e1b9-132">Request</span></span>
<span data-ttu-id="0e1b9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="0e1b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e1b9-134">Response</span></span>
<span data-ttu-id="0e1b9-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-135">The following is an example of the response.</span></span> <span data-ttu-id="0e1b9-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0e1b9-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e1b9-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->