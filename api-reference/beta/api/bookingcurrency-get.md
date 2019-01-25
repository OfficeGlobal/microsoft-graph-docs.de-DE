---
title: Abrufen von bookingCurrency
description: Rufen Sie die Eigenschaften eines BookingCurrency-Objekts, das für ein Microsoft Bookings Unternehmen verfügbar ist.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b4fd1cf854d84001d58a64dac18ca7fb276e6efa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524226"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="fd096-103">Abrufen von bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="fd096-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd096-104">Rufen Sie die Eigenschaften eines [BookingCurrency](../resources/bookingcurrency.md) -Objekts, das für ein Microsoft Bookings Unternehmen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="fd096-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="fd096-105">Verwenden Sie die **Id** -Eigenschaft, die der Währungscode ist, um die Währung anzugeben.</span><span class="sxs-lookup"><span data-stu-id="fd096-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd096-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd096-106">Permissions</span></span>
<span data-ttu-id="fd096-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd096-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd096-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd096-109">Permission type</span></span>      | <span data-ttu-id="fd096-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd096-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd096-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd096-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fd096-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="fd096-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fd096-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd096-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd096-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd096-114">Not supported.</span></span>   |
|<span data-ttu-id="fd096-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd096-115">Application</span></span> | <span data-ttu-id="fd096-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd096-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fd096-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd096-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd096-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd096-118">Optional query parameters</span></span>
<span data-ttu-id="fd096-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd096-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd096-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd096-120">Request headers</span></span>
| <span data-ttu-id="fd096-121">Name</span><span class="sxs-lookup"><span data-stu-id="fd096-121">Name</span></span>      |<span data-ttu-id="fd096-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd096-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd096-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd096-123">Authorization</span></span>  | <span data-ttu-id="fd096-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fd096-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd096-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd096-125">Request body</span></span>
<span data-ttu-id="fd096-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd096-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fd096-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd096-127">Response</span></span>
<span data-ttu-id="fd096-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingCurrency](../resources/bookingcurrency.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fd096-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd096-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd096-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd096-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd096-130">Request</span></span>
<span data-ttu-id="fd096-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd096-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="fd096-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd096-132">Response</span></span>
<span data-ttu-id="fd096-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd096-133">The following is an example of the response.</span></span> <span data-ttu-id="fd096-134">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="fd096-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fd096-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd096-135">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcurrency-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
