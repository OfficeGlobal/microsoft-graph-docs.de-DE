---
title: 'BookingBusiness: Veröffentlichen'
description: Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden zur Verfügung.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 11d8bea864772c0bcc4365c056973fac782add5d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508657"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="f8d12-103">BookingBusiness: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="f8d12-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8d12-104">Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="f8d12-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="f8d12-105">**IsPublished** -Eigenschaft auf True festgelegt, und **PublicUrl** -Eigenschaft, um die URL der Seite planen.</span><span class="sxs-lookup"><span data-stu-id="f8d12-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8d12-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8d12-106">Permissions</span></span>
<span data-ttu-id="f8d12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8d12-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8d12-109">Permission type</span></span>      | <span data-ttu-id="f8d12-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8d12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8d12-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8d12-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f8d12-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f8d12-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f8d12-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8d12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8d12-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8d12-114">Not supported.</span></span>   |
|<span data-ttu-id="f8d12-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8d12-115">Application</span></span> | <span data-ttu-id="f8d12-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8d12-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f8d12-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8d12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="f8d12-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8d12-118">Request headers</span></span>
| <span data-ttu-id="f8d12-119">Name</span><span class="sxs-lookup"><span data-stu-id="f8d12-119">Name</span></span>       | <span data-ttu-id="f8d12-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8d12-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8d12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8d12-121">Authorization</span></span>  | <span data-ttu-id="f8d12-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f8d12-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8d12-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8d12-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f8d12-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8d12-124">Response</span></span>
<span data-ttu-id="f8d12-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8d12-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8d12-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8d12-127">Example</span></span>
<span data-ttu-id="f8d12-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f8d12-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8d12-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8d12-129">Request</span></span>
<span data-ttu-id="f8d12-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8d12-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="f8d12-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8d12-131">Response</span></span>
<span data-ttu-id="f8d12-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8d12-132">The following is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
