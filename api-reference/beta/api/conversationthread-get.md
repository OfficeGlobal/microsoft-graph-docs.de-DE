---
title: conversationThread abrufen
description: 'Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 25889fad4dc60cbd69ee4e87ca8a7f4406f9e6f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935752"
---
# <a name="get-conversationthread"></a><span data-ttu-id="ad405-104">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="ad405-104">Get conversationThread</span></span>

> <span data-ttu-id="ad405-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ad405-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad405-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad405-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad405-p103">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="ad405-p103">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="ad405-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ad405-109">Permissions</span></span>
<span data-ttu-id="ad405-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad405-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad405-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ad405-112">Permission type</span></span>      | <span data-ttu-id="ad405-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ad405-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad405-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ad405-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ad405-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad405-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="ad405-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ad405-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad405-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad405-117">Not supported.</span></span>    |
|<span data-ttu-id="ad405-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ad405-118">Application</span></span> | <span data-ttu-id="ad405-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad405-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad405-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad405-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad405-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ad405-121">Optional query parameters</span></span>
<span data-ttu-id="ad405-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ad405-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad405-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad405-123">Request headers</span></span>
| <span data-ttu-id="ad405-124">Header</span><span class="sxs-lookup"><span data-stu-id="ad405-124">Header</span></span>       | <span data-ttu-id="ad405-125">Wert</span><span class="sxs-lookup"><span data-stu-id="ad405-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad405-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad405-126">Authorization</span></span>  | <span data-ttu-id="ad405-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad405-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad405-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad405-129">Request body</span></span>
<span data-ttu-id="ad405-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ad405-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad405-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad405-131">Response</span></span>

<span data-ttu-id="ad405-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad405-132">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad405-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad405-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad405-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad405-134">Request</span></span>
<span data-ttu-id="ad405-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ad405-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="ad405-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad405-136">Response</span></span>
<span data-ttu-id="ad405-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad405-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
