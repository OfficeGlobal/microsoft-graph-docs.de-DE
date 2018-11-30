---
title: conversationThread abrufen
description: 'Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
ms.openlocfilehash: b9a99be2e44b7639fe9a44b475bdf0161efa303c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059284"
---
# <a name="get-conversationthread"></a><span data-ttu-id="a5562-104">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="a5562-104">Get conversationThread</span></span>

> <span data-ttu-id="a5562-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a5562-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5562-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5562-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5562-p103">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="a5562-p103">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="a5562-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a5562-109">Permissions</span></span>
<span data-ttu-id="a5562-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5562-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5562-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5562-112">Permission type</span></span>      | <span data-ttu-id="a5562-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5562-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5562-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5562-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a5562-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5562-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="a5562-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5562-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5562-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5562-117">Not supported.</span></span>    |
|<span data-ttu-id="a5562-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5562-118">Application</span></span> | <span data-ttu-id="a5562-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5562-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5562-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5562-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5562-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a5562-121">Optional query parameters</span></span>
<span data-ttu-id="a5562-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a5562-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5562-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5562-123">Request headers</span></span>
| <span data-ttu-id="a5562-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5562-124">Header</span></span>       | <span data-ttu-id="a5562-125">Wert</span><span class="sxs-lookup"><span data-stu-id="a5562-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5562-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5562-126">Authorization</span></span>  | <span data-ttu-id="a5562-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a5562-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5562-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5562-129">Request body</span></span>
<span data-ttu-id="a5562-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a5562-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5562-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5562-131">Response</span></span>

<span data-ttu-id="a5562-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5562-132">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5562-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5562-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5562-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5562-134">Request</span></span>
<span data-ttu-id="a5562-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5562-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="a5562-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5562-136">Response</span></span>
<span data-ttu-id="a5562-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5562-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
