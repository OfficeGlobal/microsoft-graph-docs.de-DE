---
title: Liste bookingCurrencies
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e08385c887b1da6972caab83da068b0e537586db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941520"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="fe630-104">Liste bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="fe630-104">List bookingCurrencies</span></span>

 > <span data-ttu-id="fe630-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe630-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe630-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe630-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="fe630-107">Abrufen einer Liste von [BookingCurrency](../resources/bookingcurrency.md) -Objekten für ein Microsoft Bookings Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="fe630-107">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe630-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe630-108">Permissions</span></span>
<span data-ttu-id="fe630-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe630-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe630-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe630-111">Permission type</span></span>      | <span data-ttu-id="fe630-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe630-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe630-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe630-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fe630-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="fe630-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fe630-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe630-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe630-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe630-116">Not supported.</span></span>   |
|<span data-ttu-id="fe630-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe630-117">Application</span></span> | <span data-ttu-id="fe630-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe630-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fe630-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe630-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe630-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fe630-120">Optional query parameters</span></span>
<span data-ttu-id="fe630-121">Diese Methode unterstützt die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort, einschließlich $count, $filter, $select, $skip und $top anpassen.</span><span class="sxs-lookup"><span data-stu-id="fe630-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe630-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe630-122">Request headers</span></span>
| <span data-ttu-id="fe630-123">Name</span><span class="sxs-lookup"><span data-stu-id="fe630-123">Name</span></span>      |<span data-ttu-id="fe630-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe630-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe630-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe630-125">Authorization</span></span>  | <span data-ttu-id="fe630-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fe630-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe630-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe630-127">Request body</span></span>
<span data-ttu-id="fe630-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fe630-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fe630-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe630-129">Response</span></span>
<span data-ttu-id="fe630-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingCurrency](../resources/bookingcurrency.md) .</span><span class="sxs-lookup"><span data-stu-id="fe630-130">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe630-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe630-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe630-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe630-132">Request</span></span>
<span data-ttu-id="fe630-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe630-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="fe630-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe630-134">Response</span></span>
<span data-ttu-id="fe630-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fe630-135">The following is an example of the response.</span></span> <span data-ttu-id="fe630-136">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="fe630-136">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="fe630-137">Alle unterstützten Währungen und Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe630-137">All of the supported currencies and properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
