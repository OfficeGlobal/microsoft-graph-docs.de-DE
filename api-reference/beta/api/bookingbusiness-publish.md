---
title: 'BookingBusiness: Veröffentlichen'
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: b3145409de1371a164d86ad1cc52ea199d245f50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060015"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="c05a4-104">BookingBusiness: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="c05a4-104">bookingBusiness: publish</span></span>

 > <span data-ttu-id="c05a4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c05a4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c05a4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c05a4-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c05a4-107">Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="c05a4-107">Make the scheduling page of this business available to external customers.</span></span> 

<span data-ttu-id="c05a4-108">**IsPublished** -Eigenschaft auf True festgelegt, und **PublicUrl** -Eigenschaft, um die URL der Seite planen.</span><span class="sxs-lookup"><span data-stu-id="c05a4-108">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="c05a4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c05a4-109">Permissions</span></span>
<span data-ttu-id="c05a4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c05a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c05a4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c05a4-112">Permission type</span></span>      | <span data-ttu-id="c05a4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c05a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c05a4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c05a4-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c05a4-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c05a4-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c05a4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c05a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c05a4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c05a4-117">Not supported.</span></span>   |
|<span data-ttu-id="c05a4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c05a4-118">Application</span></span> | <span data-ttu-id="c05a4-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c05a4-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="c05a4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c05a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="c05a4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c05a4-121">Request headers</span></span>
| <span data-ttu-id="c05a4-122">Name</span><span class="sxs-lookup"><span data-stu-id="c05a4-122">Name</span></span>       | <span data-ttu-id="c05a4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c05a4-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c05a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c05a4-124">Authorization</span></span>  | <span data-ttu-id="c05a4-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c05a4-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c05a4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c05a4-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c05a4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c05a4-127">Response</span></span>
<span data-ttu-id="c05a4-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c05a4-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c05a4-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c05a4-130">Example</span></span>
<span data-ttu-id="c05a4-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c05a4-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c05a4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c05a4-132">Request</span></span>
<span data-ttu-id="c05a4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c05a4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="c05a4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c05a4-134">Response</span></span>
<span data-ttu-id="c05a4-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c05a4-135">The following is an example of the response.</span></span> 
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->