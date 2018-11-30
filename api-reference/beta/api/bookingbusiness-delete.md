---
title: BookingBusiness löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: d920414bb73f506c4e94cb973642c124544fc1bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059660"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="1f20b-104">BookingBusiness löschen</span><span class="sxs-lookup"><span data-stu-id="1f20b-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="1f20b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f20b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f20b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f20b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1f20b-107">Löscht ein Objekt [BookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="1f20b-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f20b-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f20b-108">Permissions</span></span>
<span data-ttu-id="1f20b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f20b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f20b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f20b-111">Permission type</span></span>      | <span data-ttu-id="1f20b-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f20b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f20b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f20b-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="1f20b-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1f20b-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1f20b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f20b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f20b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f20b-116">Not supported.</span></span>   |
|<span data-ttu-id="1f20b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f20b-117">Application</span></span> | <span data-ttu-id="1f20b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f20b-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1f20b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f20b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="1f20b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f20b-120">Request headers</span></span>
| <span data-ttu-id="1f20b-121">Name</span><span class="sxs-lookup"><span data-stu-id="1f20b-121">Name</span></span>       | <span data-ttu-id="1f20b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f20b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1f20b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f20b-123">Authorization</span></span>  | <span data-ttu-id="1f20b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1f20b-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f20b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f20b-125">Request body</span></span>
<span data-ttu-id="1f20b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f20b-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1f20b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f20b-127">Response</span></span>
<span data-ttu-id="1f20b-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f20b-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f20b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f20b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f20b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f20b-131">Request</span></span>
<span data-ttu-id="1f20b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f20b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="1f20b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f20b-133">Response</span></span>
<span data-ttu-id="1f20b-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f20b-134">The following is an example of the response.</span></span> 
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->