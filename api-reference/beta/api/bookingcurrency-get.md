---
title: Abrufen von bookingCurrency
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 14238d40dc61b64ccca976830c68d093f401e214
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059695"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="57176-104">Abrufen von bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="57176-104">Get bookingCurrency</span></span>

 > <span data-ttu-id="57176-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="57176-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57176-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57176-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="57176-107">Rufen Sie die Eigenschaften eines [BookingCurrency](../resources/bookingcurrency.md) -Objekts, das für ein Microsoft Bookings Unternehmen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="57176-107">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="57176-108">Verwenden Sie die **Id** -Eigenschaft, die der Währungscode ist, um die Währung anzugeben.</span><span class="sxs-lookup"><span data-stu-id="57176-108">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="57176-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="57176-109">Permissions</span></span>
<span data-ttu-id="57176-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57176-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57176-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57176-112">Permission type</span></span>      | <span data-ttu-id="57176-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57176-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57176-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57176-114">Delegated (work or school account)</span></span> | <span data-ttu-id="57176-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="57176-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="57176-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57176-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57176-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57176-117">Not supported.</span></span>   |
|<span data-ttu-id="57176-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57176-118">Application</span></span> | <span data-ttu-id="57176-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57176-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="57176-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57176-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57176-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="57176-121">Optional query parameters</span></span>
<span data-ttu-id="57176-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="57176-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57176-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57176-123">Request headers</span></span>
| <span data-ttu-id="57176-124">Name</span><span class="sxs-lookup"><span data-stu-id="57176-124">Name</span></span>      |<span data-ttu-id="57176-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57176-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57176-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="57176-126">Authorization</span></span>  | <span data-ttu-id="57176-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="57176-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="57176-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57176-128">Request body</span></span>
<span data-ttu-id="57176-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="57176-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="57176-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="57176-130">Response</span></span>
<span data-ttu-id="57176-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingCurrency](../resources/bookingcurrency.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="57176-131">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57176-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57176-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57176-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57176-133">Request</span></span>
<span data-ttu-id="57176-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57176-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="57176-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="57176-135">Response</span></span>
<span data-ttu-id="57176-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="57176-136">The following is an example of the response.</span></span> <span data-ttu-id="57176-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="57176-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="57176-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57176-138">All of the properties will be returned from an actual call.</span></span>
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