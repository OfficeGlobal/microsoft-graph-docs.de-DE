---
title: 'BookingBusiness: Aufheben der Veröffentlichung'
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: fc2556b62ab3b9a32ca278704864265c2de4d25e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838787"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="784fa-104">BookingBusiness: Aufheben der Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="784fa-104">bookingBusiness: unpublish</span></span>

 > <span data-ttu-id="784fa-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="784fa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="784fa-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="784fa-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="784fa-107">Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="784fa-107">Make the scheduling page of this business not available to external customers.</span></span> 

<span data-ttu-id="784fa-108">**IsPublished** -Eigenschaft auf False und **PublicUrl** -Eigenschaft auf null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="784fa-108">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="784fa-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="784fa-109">Permissions</span></span>
<span data-ttu-id="784fa-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="784fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="784fa-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="784fa-112">Permission type</span></span>      | <span data-ttu-id="784fa-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="784fa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="784fa-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="784fa-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="784fa-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="784fa-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="784fa-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="784fa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="784fa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="784fa-117">Not supported.</span></span>   |
|<span data-ttu-id="784fa-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="784fa-118">Application</span></span> | <span data-ttu-id="784fa-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="784fa-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="784fa-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="784fa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="784fa-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="784fa-121">Request headers</span></span>
| <span data-ttu-id="784fa-122">Name</span><span class="sxs-lookup"><span data-stu-id="784fa-122">Name</span></span>       | <span data-ttu-id="784fa-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="784fa-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="784fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="784fa-124">Authorization</span></span>  | <span data-ttu-id="784fa-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="784fa-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="784fa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="784fa-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="784fa-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="784fa-127">Response</span></span>
<span data-ttu-id="784fa-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="784fa-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="784fa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="784fa-130">Example</span></span>
<span data-ttu-id="784fa-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="784fa-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="784fa-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="784fa-132">Request</span></span>
<span data-ttu-id="784fa-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="784fa-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="784fa-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="784fa-134">Response</span></span>
<span data-ttu-id="784fa-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="784fa-135">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
