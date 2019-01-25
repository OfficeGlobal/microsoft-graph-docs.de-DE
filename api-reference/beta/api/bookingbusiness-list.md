---
title: Liste bookingBusinesses
description: Rufen Sie eine Auflistung von Bookingbusiness-Objekten, die erstellt wurde, für den Mandanten.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8018b8ac7f9d2e5f74e4233dbc36c2a6faa2d9a8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523155"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="70c91-103">Liste bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="70c91-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70c91-104">Rufen Sie eine Auflistung von [Bookingbusiness](../resources/bookingbusiness.md) -Objekten, die erstellt wurde, für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70c91-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="70c91-105">Dieser Vorgang gibt nur die **Id** und **DisplayName** jedes Buchungen Unternehmens in der Auflistung zurück.</span><span class="sxs-lookup"><span data-stu-id="70c91-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="70c91-106">Unter Leistungsgesichtspunkten gibt es keine anderen Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="70c91-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="70c91-107">Sie können die anderen Eigenschaften eines Unternehmens Buchungen abrufen, indem dessen **Id** angeben, in einem Vorgang [erhalten möchten](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="70c91-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="70c91-108">Sie können auch für Unternehmen Buchungen Abfragen, durch Angeben einer Zeichenfolge in einer `query` Parameter untergeordnete Zeichenfolgen Übereinstimmung zwischen dem Unternehmen eines Mandanten liegen.</span><span class="sxs-lookup"><span data-stu-id="70c91-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="70c91-109">Unten finden Sie ein [Beispiel](#request-2).</span><span class="sxs-lookup"><span data-stu-id="70c91-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="70c91-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70c91-110">Permissions</span></span>
<span data-ttu-id="70c91-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c91-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70c91-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70c91-113">Permission type</span></span>      | <span data-ttu-id="70c91-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70c91-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70c91-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70c91-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="70c91-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="70c91-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="70c91-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70c91-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70c91-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70c91-118">Not supported.</span></span>   |
|<span data-ttu-id="70c91-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70c91-119">Application</span></span> | <span data-ttu-id="70c91-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70c91-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="70c91-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c91-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70c91-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="70c91-122">Optional query parameters</span></span>
<span data-ttu-id="70c91-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c91-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="70c91-124">Diese Methode unterstützt die `query` -Parameter der akzeptiert einen String-Wert.</span><span class="sxs-lookup"><span data-stu-id="70c91-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="70c91-125">Dieser Parameter beschränkt das Abrufen der Ergebnisse an Unternehmen, die der angegebenen Zeichenfolge entsprechen.</span><span class="sxs-lookup"><span data-stu-id="70c91-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="70c91-126">Sehen Sie ein [Beispiel](#request-2) unten ein.</span><span class="sxs-lookup"><span data-stu-id="70c91-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="70c91-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70c91-127">Request headers</span></span>
| <span data-ttu-id="70c91-128">Name</span><span class="sxs-lookup"><span data-stu-id="70c91-128">Name</span></span>      |<span data-ttu-id="70c91-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c91-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70c91-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="70c91-130">Authorization</span></span>  | <span data-ttu-id="70c91-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="70c91-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c91-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70c91-132">Request body</span></span>
<span data-ttu-id="70c91-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="70c91-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="70c91-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c91-134">Response</span></span>
<span data-ttu-id="70c91-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="70c91-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70c91-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70c91-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="70c91-137">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="70c91-137">Request 1</span></span>
<span data-ttu-id="70c91-138">Im folgenden Beispiel wird die Buchungen Unternehmen in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70c91-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="70c91-139">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="70c91-139">Response 1</span></span>
<span data-ttu-id="70c91-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c91-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="70c91-141">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="70c91-141">Request 2</span></span>
<span data-ttu-id="70c91-142">Das folgende Beispiel zeigt, wie Sie mit der `query` Parameter zum Abrufen von mindestens einen übereinstimmender Buchungen Unternehmen in den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70c91-142">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="70c91-143">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="70c91-143">Response 2</span></span>
<span data-ttu-id="70c91-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c91-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
