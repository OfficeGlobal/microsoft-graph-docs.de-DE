---
title: Beiträge auflisten
description: 'Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
ms.openlocfilehash: 35c4c178b02cb700ab21a324c29a4522203fad19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017584"
---
# <a name="list-posts"></a><span data-ttu-id="594d7-104">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="594d7-104">List posts</span></span>

<span data-ttu-id="594d7-p102">Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="594d7-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="594d7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="594d7-107">Permissions</span></span>
<span data-ttu-id="594d7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="594d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="594d7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="594d7-110">Permission type</span></span>      | <span data-ttu-id="594d7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="594d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="594d7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="594d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="594d7-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="594d7-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="594d7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="594d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="594d7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="594d7-115">Not supported.</span></span>    |
|<span data-ttu-id="594d7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="594d7-116">Application</span></span> | <span data-ttu-id="594d7-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="594d7-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="594d7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="594d7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="594d7-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="594d7-119">Optional query parameters</span></span>
<span data-ttu-id="594d7-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="594d7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="594d7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="594d7-121">Request headers</span></span>
| <span data-ttu-id="594d7-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="594d7-122">Header</span></span>       | <span data-ttu-id="594d7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="594d7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="594d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="594d7-124">Authorization</span></span>  | <span data-ttu-id="594d7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="594d7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="594d7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="594d7-127">Request body</span></span>
<span data-ttu-id="594d7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="594d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="594d7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="594d7-129">Response</span></span>

<span data-ttu-id="594d7-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Post](../resources/post.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="594d7-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="594d7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="594d7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="594d7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="594d7-132">Request</span></span>
<span data-ttu-id="594d7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="594d7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="594d7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="594d7-134">Response</span></span>
<span data-ttu-id="594d7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="594d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->