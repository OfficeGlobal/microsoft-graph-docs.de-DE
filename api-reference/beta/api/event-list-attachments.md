---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs attachment abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cf092595f558d3aa1529023029ce84c6f2a4cb87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524009"
---
# <a name="list-attachments"></a><span data-ttu-id="14cd6-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="14cd6-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14cd6-104">Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="14cd6-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="14cd6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="14cd6-105">Permissions</span></span>

<span data-ttu-id="14cd6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14cd6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14cd6-108">Permission type</span></span>      | <span data-ttu-id="14cd6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14cd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14cd6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14cd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14cd6-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14cd6-111">Calendars.Read</span></span>    |
|<span data-ttu-id="14cd6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14cd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14cd6-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14cd6-113">Calendars.Read</span></span>    |
|<span data-ttu-id="14cd6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14cd6-114">Application</span></span> | <span data-ttu-id="14cd6-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14cd6-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="14cd6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14cd6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="14cd6-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="14cd6-117">Optional query parameters</span></span>

<span data-ttu-id="14cd6-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="14cd6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="14cd6-119">Insbesondere, können Sie mithilfe der `$expand` Abfragen Parameter, um alle für das Ereignis Anlagen Inline mit dem Rest der Ereigniseigenschaften enthalten.</span><span class="sxs-lookup"><span data-stu-id="14cd6-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="14cd6-120">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="14cd6-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="14cd6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14cd6-121">Request headers</span></span>

| <span data-ttu-id="14cd6-122">Name</span><span class="sxs-lookup"><span data-stu-id="14cd6-122">Name</span></span>       | <span data-ttu-id="14cd6-123">Typ</span><span class="sxs-lookup"><span data-stu-id="14cd6-123">Type</span></span> | <span data-ttu-id="14cd6-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14cd6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14cd6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14cd6-125">Authorization</span></span>  | <span data-ttu-id="14cd6-126">string</span><span class="sxs-lookup"><span data-stu-id="14cd6-126">string</span></span>  | <span data-ttu-id="14cd6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="14cd6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14cd6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14cd6-129">Request body</span></span>

<span data-ttu-id="14cd6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="14cd6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14cd6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="14cd6-131">Response</span></span>

<span data-ttu-id="14cd6-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14cd6-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14cd6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14cd6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="14cd6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14cd6-134">Request</span></span>

<span data-ttu-id="14cd6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14cd6-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="14cd6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="14cd6-136">Response</span></span>

<span data-ttu-id="14cd6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14cd6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
