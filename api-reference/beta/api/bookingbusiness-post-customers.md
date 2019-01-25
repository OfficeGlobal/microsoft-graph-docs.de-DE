---
title: Erstellen von bookingCustomer
description: Erstellen eines neuen BookingCustomer-Objekts.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4557d65edf4727659fdae94599c0796fc940ed1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523960"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="71ab7-103">Erstellen von bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="71ab7-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71ab7-104">Erstellen eines neuen [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71ab7-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71ab7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71ab7-105">Permissions</span></span>
<span data-ttu-id="71ab7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ab7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71ab7-108">Permission type</span></span>      | <span data-ttu-id="71ab7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71ab7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71ab7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71ab7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="71ab7-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="71ab7-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="71ab7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71ab7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71ab7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71ab7-113">Not supported.</span></span>   |
|<span data-ttu-id="71ab7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71ab7-114">Application</span></span> | <span data-ttu-id="71ab7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71ab7-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="71ab7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71ab7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="71ab7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71ab7-117">Request headers</span></span>
| <span data-ttu-id="71ab7-118">Name</span><span class="sxs-lookup"><span data-stu-id="71ab7-118">Name</span></span>       | <span data-ttu-id="71ab7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71ab7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71ab7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71ab7-120">Authorization</span></span>  | <span data-ttu-id="71ab7-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="71ab7-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ab7-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71ab7-122">Request body</span></span>
<span data-ttu-id="71ab7-123">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71ab7-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="71ab7-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="71ab7-124">Response</span></span>
<span data-ttu-id="71ab7-125">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingCustomer](../resources/bookingcustomer.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="71ab7-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ab7-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71ab7-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71ab7-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71ab7-127">Request</span></span>
<span data-ttu-id="71ab7-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71ab7-128">The following is an example of the request.</span></span>
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
<span data-ttu-id="71ab7-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingCustomer](../resources/bookingcustomer.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71ab7-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71ab7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="71ab7-130">Response</span></span>
<span data-ttu-id="71ab7-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71ab7-131">The following is an example of the response.</span></span> <span data-ttu-id="71ab7-132">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="71ab7-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="71ab7-133">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71ab7-133">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
