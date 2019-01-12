---
title: Liste bookingBusinesses
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 51b8e049b45542de9940168c994bed8fbd273b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951453"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d8666-104">Liste bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="d8666-104">List bookingBusinesses</span></span>

 > <span data-ttu-id="d8666-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8666-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8666-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8666-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d8666-107">Rufen Sie eine Auflistung von [Bookingbusiness](../resources/bookingbusiness.md) -Objekten, die erstellt wurde, für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d8666-107">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span> 

<span data-ttu-id="d8666-108">Dieser Vorgang gibt nur die **Id** und **DisplayName** jedes Buchungen Unternehmens in der Auflistung zurück.</span><span class="sxs-lookup"><span data-stu-id="d8666-108">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d8666-109">Unter Leistungsgesichtspunkten gibt es keine anderen Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d8666-109">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d8666-110">Sie können die anderen Eigenschaften eines Unternehmens Buchungen abrufen, indem dessen **Id** angeben, in einem Vorgang [erhalten möchten](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d8666-110">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d8666-111">Sie können auch für Unternehmen Buchungen Abfragen, durch Angeben einer Zeichenfolge in einer `query` Parameter untergeordnete Zeichenfolgen Übereinstimmung zwischen dem Unternehmen eines Mandanten liegen.</span><span class="sxs-lookup"><span data-stu-id="d8666-111">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d8666-112">Sehen Sie ein [Beispiel](#request-2) unten.</span><span class="sxs-lookup"><span data-stu-id="d8666-112">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d8666-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d8666-113">Permissions</span></span>
<span data-ttu-id="d8666-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8666-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8666-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d8666-116">Permission type</span></span>      | <span data-ttu-id="d8666-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d8666-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8666-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d8666-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d8666-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d8666-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d8666-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d8666-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8666-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8666-121">Not supported.</span></span>   |
|<span data-ttu-id="d8666-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d8666-122">Application</span></span> | <span data-ttu-id="d8666-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8666-123">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="d8666-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8666-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8666-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d8666-125">Optional query parameters</span></span>
<span data-ttu-id="d8666-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d8666-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d8666-127">Diese Methode unterstützt die `query` -Parameter der akzeptiert einen String-Wert.</span><span class="sxs-lookup"><span data-stu-id="d8666-127">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d8666-128">Dieser Parameter beschränkt das Abrufen der Ergebnisse an Unternehmen, die der angegebenen Zeichenfolge entsprechen.</span><span class="sxs-lookup"><span data-stu-id="d8666-128">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d8666-129">Sehen Sie ein [Beispiel](#request-2) unten ein.</span><span class="sxs-lookup"><span data-stu-id="d8666-129">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d8666-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d8666-130">Request headers</span></span>
| <span data-ttu-id="d8666-131">Name</span><span class="sxs-lookup"><span data-stu-id="d8666-131">Name</span></span>      |<span data-ttu-id="d8666-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8666-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8666-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8666-133">Authorization</span></span>  | <span data-ttu-id="d8666-134">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d8666-134">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8666-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d8666-135">Request body</span></span>
<span data-ttu-id="d8666-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d8666-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d8666-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8666-137">Response</span></span>
<span data-ttu-id="d8666-138">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="d8666-138">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8666-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d8666-139">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d8666-140">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="d8666-140">Request 1</span></span>
<span data-ttu-id="d8666-141">Im folgenden Beispiel wird die Buchungen Unternehmen in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d8666-141">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="d8666-142">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="d8666-142">Response 1</span></span>
<span data-ttu-id="d8666-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d8666-143">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="d8666-144">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="d8666-144">Request 2</span></span>
<span data-ttu-id="d8666-145">Das folgende Beispiel zeigt, wie Sie mit der `query` Parameter zum Abrufen von mindestens einen übereinstimmender Buchungen Unternehmen in den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d8666-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="d8666-146">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="d8666-146">Response 2</span></span>
<span data-ttu-id="d8666-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d8666-147">The following is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
