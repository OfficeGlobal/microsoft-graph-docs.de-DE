---
title: BookingBusiness löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 273c3f3578653e457122b2bf045eb54644ea6b08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849917"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="f7152-104">BookingBusiness löschen</span><span class="sxs-lookup"><span data-stu-id="f7152-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="f7152-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7152-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7152-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7152-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f7152-107">Löscht ein Objekt [BookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="f7152-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7152-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7152-108">Permissions</span></span>
<span data-ttu-id="f7152-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7152-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7152-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7152-111">Permission type</span></span>      | <span data-ttu-id="f7152-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7152-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7152-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7152-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7152-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f7152-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f7152-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7152-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7152-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7152-116">Not supported.</span></span>   |
|<span data-ttu-id="f7152-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7152-117">Application</span></span> | <span data-ttu-id="f7152-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7152-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f7152-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7152-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="f7152-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7152-120">Request headers</span></span>
| <span data-ttu-id="f7152-121">Name</span><span class="sxs-lookup"><span data-stu-id="f7152-121">Name</span></span>       | <span data-ttu-id="f7152-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7152-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7152-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7152-123">Authorization</span></span>  | <span data-ttu-id="f7152-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f7152-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7152-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7152-125">Request body</span></span>
<span data-ttu-id="f7152-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7152-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f7152-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7152-127">Response</span></span>
<span data-ttu-id="f7152-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7152-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7152-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7152-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7152-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7152-131">Request</span></span>
<span data-ttu-id="f7152-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7152-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="f7152-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7152-133">Response</span></span>
<span data-ttu-id="f7152-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7152-134">The following is an example of the response.</span></span> 
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
