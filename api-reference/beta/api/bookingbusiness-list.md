---
title: Liste bookingBusinesses
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 270bda6aca601951ea56a9ddf9364d1459496699
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849210"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="f0164-104">Liste bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="f0164-104">List bookingBusinesses</span></span>

 > <span data-ttu-id="f0164-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f0164-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0164-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0164-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f0164-107">Rufen Sie eine Auflistung von [Bookingbusiness](../resources/bookingbusiness.md) -Objekten, die erstellt wurde, für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f0164-107">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span> 

<span data-ttu-id="f0164-108">Dieser Vorgang gibt nur die **Id** und **DisplayName** jedes Buchungen Unternehmens in der Auflistung zurück.</span><span class="sxs-lookup"><span data-stu-id="f0164-108">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="f0164-109">Unter Leistungsgesichtspunkten gibt es keine anderen Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f0164-109">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="f0164-110">Sie können die anderen Eigenschaften eines Unternehmens Buchungen abrufen, indem dessen **Id** angeben, in einem Vorgang [erhalten möchten](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="f0164-110">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="f0164-111">Sie können auch für Unternehmen Buchungen Abfragen, durch Angeben einer Zeichenfolge in einer `query` Parameter untergeordnete Zeichenfolgen Übereinstimmung zwischen dem Unternehmen eines Mandanten liegen.</span><span class="sxs-lookup"><span data-stu-id="f0164-111">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="f0164-112">Sehen Sie ein [Beispiel](#request-2) unten.</span><span class="sxs-lookup"><span data-stu-id="f0164-112">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="f0164-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0164-113">Permissions</span></span>
<span data-ttu-id="f0164-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0164-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0164-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0164-116">Permission type</span></span>      | <span data-ttu-id="f0164-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f0164-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0164-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0164-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="f0164-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f0164-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f0164-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0164-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0164-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0164-121">Not supported.</span></span>   |
|<span data-ttu-id="f0164-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0164-122">Application</span></span> | <span data-ttu-id="f0164-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0164-123">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f0164-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0164-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0164-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f0164-125">Optional query parameters</span></span>
<span data-ttu-id="f0164-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f0164-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f0164-127">Diese Methode unterstützt die `query` -Parameter der akzeptiert einen String-Wert.</span><span class="sxs-lookup"><span data-stu-id="f0164-127">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="f0164-128">Dieser Parameter beschränkt das Abrufen der Ergebnisse an Unternehmen, die der angegebenen Zeichenfolge entsprechen.</span><span class="sxs-lookup"><span data-stu-id="f0164-128">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="f0164-129">Sehen Sie ein [Beispiel](#request-2) unten ein.</span><span class="sxs-lookup"><span data-stu-id="f0164-129">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="f0164-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0164-130">Request headers</span></span>
| <span data-ttu-id="f0164-131">Name</span><span class="sxs-lookup"><span data-stu-id="f0164-131">Name</span></span>      |<span data-ttu-id="f0164-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0164-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0164-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0164-133">Authorization</span></span>  | <span data-ttu-id="f0164-134">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f0164-134">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0164-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0164-135">Request body</span></span>
<span data-ttu-id="f0164-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f0164-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f0164-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0164-137">Response</span></span>
<span data-ttu-id="f0164-138">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="f0164-138">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0164-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0164-139">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f0164-140">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="f0164-140">Request 1</span></span>
<span data-ttu-id="f0164-141">Im folgenden Beispiel wird die Buchungen Unternehmen in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f0164-141">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="f0164-142">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="f0164-142">Response 1</span></span>
<span data-ttu-id="f0164-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f0164-143">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="f0164-144">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="f0164-144">Request 2</span></span>
<span data-ttu-id="f0164-145">Das folgende Beispiel zeigt, wie Sie mit der `query` Parameter zum Abrufen von mindestens einen übereinstimmender Buchungen Unternehmen in den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f0164-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="f0164-146">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="f0164-146">Response 2</span></span>
<span data-ttu-id="f0164-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f0164-147">The following is an example of the response.</span></span>
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
