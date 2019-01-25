---
title: BookingService löschen
description: Löschen eines BookingService-Objekts in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a541796fbfa500cc6d99205598042818b4aa47ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517036"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="de357-103">BookingService löschen</span><span class="sxs-lookup"><span data-stu-id="de357-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de357-104">Löschen eines [BookingService](../resources/bookingservice.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="de357-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="de357-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de357-105">Permissions</span></span>
<span data-ttu-id="de357-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de357-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de357-108">Permission type</span></span>      | <span data-ttu-id="de357-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de357-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de357-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de357-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="de357-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="de357-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="de357-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de357-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de357-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de357-113">Not supported.</span></span>   |
|<span data-ttu-id="de357-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de357-114">Application</span></span> | <span data-ttu-id="de357-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de357-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="de357-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de357-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="de357-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de357-117">Request headers</span></span>
| <span data-ttu-id="de357-118">Name</span><span class="sxs-lookup"><span data-stu-id="de357-118">Name</span></span>       | <span data-ttu-id="de357-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de357-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de357-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de357-120">Authorization</span></span>  | <span data-ttu-id="de357-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="de357-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="de357-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de357-122">Request body</span></span>
<span data-ttu-id="de357-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="de357-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="de357-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="de357-124">Response</span></span>
<span data-ttu-id="de357-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de357-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de357-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de357-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de357-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de357-128">Request</span></span>
<span data-ttu-id="de357-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de357-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="de357-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="de357-130">Response</span></span>
<span data-ttu-id="de357-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="de357-131">The following is an example of the response.</span></span> <span data-ttu-id="de357-132">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="de357-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="de357-133">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de357-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
