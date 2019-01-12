---
title: Abrufen von bookingCurrency
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f408ab0110de5124bb4154d0107c801b026de29a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926351"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="dec9b-104">Abrufen von bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="dec9b-104">Get bookingCurrency</span></span>

 > <span data-ttu-id="dec9b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dec9b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dec9b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dec9b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="dec9b-107">Rufen Sie die Eigenschaften eines [BookingCurrency](../resources/bookingcurrency.md) -Objekts, das für ein Microsoft Bookings Unternehmen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="dec9b-107">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="dec9b-108">Verwenden Sie die **Id** -Eigenschaft, die der Währungscode ist, um die Währung anzugeben.</span><span class="sxs-lookup"><span data-stu-id="dec9b-108">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="dec9b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dec9b-109">Permissions</span></span>
<span data-ttu-id="dec9b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec9b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec9b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dec9b-112">Permission type</span></span>      | <span data-ttu-id="dec9b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dec9b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dec9b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dec9b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dec9b-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="dec9b-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="dec9b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dec9b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dec9b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec9b-117">Not supported.</span></span>   |
|<span data-ttu-id="dec9b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dec9b-118">Application</span></span> | <span data-ttu-id="dec9b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec9b-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="dec9b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec9b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dec9b-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dec9b-121">Optional query parameters</span></span>
<span data-ttu-id="dec9b-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dec9b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dec9b-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dec9b-123">Request headers</span></span>
| <span data-ttu-id="dec9b-124">Name</span><span class="sxs-lookup"><span data-stu-id="dec9b-124">Name</span></span>      |<span data-ttu-id="dec9b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dec9b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dec9b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dec9b-126">Authorization</span></span>  | <span data-ttu-id="dec9b-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dec9b-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dec9b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dec9b-128">Request body</span></span>
<span data-ttu-id="dec9b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dec9b-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dec9b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec9b-130">Response</span></span>
<span data-ttu-id="dec9b-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingCurrency](../resources/bookingcurrency.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dec9b-131">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dec9b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dec9b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dec9b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec9b-133">Request</span></span>
<span data-ttu-id="dec9b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dec9b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="dec9b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec9b-135">Response</span></span>
<span data-ttu-id="dec9b-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dec9b-136">The following is an example of the response.</span></span> <span data-ttu-id="dec9b-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="dec9b-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dec9b-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dec9b-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
