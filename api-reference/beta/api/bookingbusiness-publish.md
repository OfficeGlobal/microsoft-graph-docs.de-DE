---
title: 'BookingBusiness: Veröffentlichen'
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33e11fac5690e66664038705b482480ef689db6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917321"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="0d367-104">BookingBusiness: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="0d367-104">bookingBusiness: publish</span></span>

 > <span data-ttu-id="0d367-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0d367-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d367-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d367-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="0d367-107">Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="0d367-107">Make the scheduling page of this business available to external customers.</span></span> 

<span data-ttu-id="0d367-108">**IsPublished** -Eigenschaft auf True festgelegt, und **PublicUrl** -Eigenschaft, um die URL der Seite planen.</span><span class="sxs-lookup"><span data-stu-id="0d367-108">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d367-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d367-109">Permissions</span></span>
<span data-ttu-id="0d367-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d367-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d367-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d367-112">Permission type</span></span>      | <span data-ttu-id="0d367-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d367-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d367-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d367-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="0d367-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0d367-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0d367-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d367-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d367-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d367-117">Not supported.</span></span>   |
|<span data-ttu-id="0d367-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d367-118">Application</span></span> | <span data-ttu-id="0d367-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d367-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="0d367-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d367-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="0d367-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d367-121">Request headers</span></span>
| <span data-ttu-id="0d367-122">Name</span><span class="sxs-lookup"><span data-stu-id="0d367-122">Name</span></span>       | <span data-ttu-id="0d367-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d367-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d367-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d367-124">Authorization</span></span>  | <span data-ttu-id="0d367-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0d367-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d367-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d367-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0d367-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d367-127">Response</span></span>
<span data-ttu-id="0d367-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d367-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d367-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d367-130">Example</span></span>
<span data-ttu-id="0d367-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0d367-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0d367-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d367-132">Request</span></span>
<span data-ttu-id="0d367-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d367-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="0d367-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d367-134">Response</span></span>
<span data-ttu-id="0d367-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0d367-135">The following is an example of the response.</span></span> 
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
