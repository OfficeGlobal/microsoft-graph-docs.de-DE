---
title: Liste bookingCurrencies
description: Abrufen einer Liste von BookingCurrency-Objekten für ein Microsoft Bookings Unternehmen verfügbar.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c29ad5780deac5e5e338052c72661f834e483054
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513221"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="414ea-103">Liste bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="414ea-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="414ea-104">Abrufen einer Liste von [BookingCurrency](../resources/bookingcurrency.md) -Objekten für ein Microsoft Bookings Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="414ea-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="414ea-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="414ea-105">Permissions</span></span>
<span data-ttu-id="414ea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="414ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="414ea-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="414ea-108">Permission type</span></span>      | <span data-ttu-id="414ea-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="414ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="414ea-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="414ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="414ea-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="414ea-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="414ea-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="414ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="414ea-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="414ea-113">Not supported.</span></span>   |
|<span data-ttu-id="414ea-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="414ea-114">Application</span></span> | <span data-ttu-id="414ea-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="414ea-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="414ea-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="414ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="414ea-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="414ea-117">Optional query parameters</span></span>
<span data-ttu-id="414ea-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort, einschließlich $count, $filter, $select, $skip und $top anpassen.</span><span class="sxs-lookup"><span data-stu-id="414ea-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="414ea-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="414ea-119">Request headers</span></span>
| <span data-ttu-id="414ea-120">Name</span><span class="sxs-lookup"><span data-stu-id="414ea-120">Name</span></span>      |<span data-ttu-id="414ea-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="414ea-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="414ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="414ea-122">Authorization</span></span>  | <span data-ttu-id="414ea-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="414ea-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="414ea-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="414ea-124">Request body</span></span>
<span data-ttu-id="414ea-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="414ea-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="414ea-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="414ea-126">Response</span></span>
<span data-ttu-id="414ea-127">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingCurrency](../resources/bookingcurrency.md) .</span><span class="sxs-lookup"><span data-stu-id="414ea-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="414ea-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="414ea-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="414ea-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="414ea-129">Request</span></span>
<span data-ttu-id="414ea-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="414ea-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="414ea-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="414ea-131">Response</span></span>
<span data-ttu-id="414ea-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="414ea-132">The following is an example of the response.</span></span> <span data-ttu-id="414ea-133">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="414ea-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="414ea-134">Alle unterstützten Währungen und Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="414ea-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
