---
title: BookingService löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7616e04c25aefedde084fc47c06d22410f9f0fee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991223"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="3db4b-104">BookingService löschen</span><span class="sxs-lookup"><span data-stu-id="3db4b-104">Delete bookingService</span></span>

 > <span data-ttu-id="3db4b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3db4b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3db4b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3db4b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="3db4b-107">Löschen eines [BookingService](../resources/bookingservice.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3db4b-107">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3db4b-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3db4b-108">Permissions</span></span>
<span data-ttu-id="3db4b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db4b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db4b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3db4b-111">Permission type</span></span>      | <span data-ttu-id="3db4b-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3db4b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db4b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3db4b-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3db4b-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3db4b-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3db4b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3db4b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db4b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3db4b-116">Not supported.</span></span>   |
|<span data-ttu-id="3db4b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3db4b-117">Application</span></span> | <span data-ttu-id="3db4b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3db4b-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3db4b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db4b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3db4b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3db4b-120">Request headers</span></span>
| <span data-ttu-id="3db4b-121">Name</span><span class="sxs-lookup"><span data-stu-id="3db4b-121">Name</span></span>       | <span data-ttu-id="3db4b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3db4b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3db4b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3db4b-123">Authorization</span></span>  | <span data-ttu-id="3db4b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3db4b-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3db4b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3db4b-125">Request body</span></span>
<span data-ttu-id="3db4b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3db4b-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3db4b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db4b-127">Response</span></span>
<span data-ttu-id="3db4b-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3db4b-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3db4b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3db4b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3db4b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db4b-131">Request</span></span>
<span data-ttu-id="3db4b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3db4b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="3db4b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db4b-133">Response</span></span>
<span data-ttu-id="3db4b-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3db4b-134">The following is an example of the response.</span></span> <span data-ttu-id="3db4b-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3db4b-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3db4b-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3db4b-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
