---
title: Erstellen von bookingCustomer
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 555723fdb4eb7bacb2c876ed3fd87eb539a5239d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922256"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="f4fe8-104">Erstellen von bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="f4fe8-104">Create bookingCustomer</span></span>

 > <span data-ttu-id="f4fe8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4fe8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f4fe8-107">Erstellen eines neuen [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-107">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4fe8-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f4fe8-108">Permissions</span></span>
<span data-ttu-id="f4fe8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4fe8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4fe8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4fe8-111">Permission type</span></span>      | <span data-ttu-id="f4fe8-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4fe8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4fe8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4fe8-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f4fe8-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f4fe8-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f4fe8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4fe8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4fe8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4fe8-116">Not supported.</span></span>   |
|<span data-ttu-id="f4fe8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4fe8-117">Application</span></span> | <span data-ttu-id="f4fe8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4fe8-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f4fe8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4fe8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="f4fe8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4fe8-120">Request headers</span></span>
| <span data-ttu-id="f4fe8-121">Name</span><span class="sxs-lookup"><span data-stu-id="f4fe8-121">Name</span></span>       | <span data-ttu-id="f4fe8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4fe8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4fe8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4fe8-123">Authorization</span></span>  | <span data-ttu-id="f4fe8-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f4fe8-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4fe8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4fe8-125">Request body</span></span>
<span data-ttu-id="f4fe8-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-126">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f4fe8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4fe8-127">Response</span></span>
<span data-ttu-id="f4fe8-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingCustomer](../resources/bookingcustomer.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-128">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4fe8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4fe8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4fe8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4fe8-130">Request</span></span>
<span data-ttu-id="f4fe8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers

Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
<span data-ttu-id="f4fe8-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-132">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f4fe8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4fe8-133">Response</span></span>
<span data-ttu-id="f4fe8-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-134">The following is an example of the response.</span></span> <span data-ttu-id="f4fe8-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f4fe8-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
