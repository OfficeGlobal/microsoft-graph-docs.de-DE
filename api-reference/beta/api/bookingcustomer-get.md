---
title: Abrufen von bookingCustomer
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 38a0fa87bc3b81c493914b14a8c35a01dad11689
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27989991"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="f5019-104">Abrufen von bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="f5019-104">Get bookingCustomer</span></span>

 > <span data-ttu-id="f5019-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f5019-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5019-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5019-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f5019-107">Rufen Sie die Eigenschaften und die Beziehungen eines [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f5019-107">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5019-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5019-108">Permissions</span></span>
<span data-ttu-id="f5019-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5019-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5019-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5019-111">Permission type</span></span>      | <span data-ttu-id="f5019-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5019-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5019-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5019-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f5019-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f5019-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f5019-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5019-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5019-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5019-116">Not supported.</span></span>   |
|<span data-ttu-id="f5019-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5019-117">Application</span></span> | <span data-ttu-id="f5019-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5019-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="f5019-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5019-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5019-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f5019-120">Optional query parameters</span></span>
<span data-ttu-id="f5019-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5019-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5019-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5019-122">Request headers</span></span>
| <span data-ttu-id="f5019-123">Name</span><span class="sxs-lookup"><span data-stu-id="f5019-123">Name</span></span>      |<span data-ttu-id="f5019-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5019-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5019-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5019-125">Authorization</span></span>  | <span data-ttu-id="f5019-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f5019-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5019-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5019-127">Request body</span></span>
<span data-ttu-id="f5019-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f5019-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f5019-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5019-129">Response</span></span>
<span data-ttu-id="f5019-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingCustomer](../resources/bookingcustomer.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f5019-130">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5019-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5019-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5019-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5019-132">Request</span></span>
<span data-ttu-id="f5019-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5019-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="f5019-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5019-134">Response</span></span>
<span data-ttu-id="f5019-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5019-135">The following is an example of the response.</span></span> <span data-ttu-id="f5019-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="f5019-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f5019-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5019-137">All of the properties will be returned from an actual call.</span></span>
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
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
