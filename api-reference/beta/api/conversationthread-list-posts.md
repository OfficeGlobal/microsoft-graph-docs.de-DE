---
title: Beiträge auflisten
description: 'Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
ms.openlocfilehash: 9253076a0232954acfdd1effad3fdb8084bba3fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061624"
---
# <a name="list-posts"></a><span data-ttu-id="ae25e-104">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="ae25e-104">List posts</span></span>

> <span data-ttu-id="ae25e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae25e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae25e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae25e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae25e-p103">Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="ae25e-p103">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae25e-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae25e-109">Permissions</span></span>
<span data-ttu-id="ae25e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae25e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae25e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae25e-112">Permission type</span></span>      | <span data-ttu-id="ae25e-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae25e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae25e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae25e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ae25e-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae25e-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="ae25e-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae25e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae25e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae25e-117">Not supported.</span></span>    |
|<span data-ttu-id="ae25e-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae25e-118">Application</span></span> | <span data-ttu-id="ae25e-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae25e-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae25e-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae25e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae25e-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ae25e-121">Optional query parameters</span></span>
<span data-ttu-id="ae25e-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ae25e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae25e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae25e-123">Request headers</span></span>
| <span data-ttu-id="ae25e-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ae25e-124">Header</span></span>       | <span data-ttu-id="ae25e-125">Wert</span><span class="sxs-lookup"><span data-stu-id="ae25e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae25e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae25e-126">Authorization</span></span>  | <span data-ttu-id="ae25e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae25e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae25e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae25e-129">Request body</span></span>
<span data-ttu-id="ae25e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ae25e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae25e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae25e-131">Response</span></span>

<span data-ttu-id="ae25e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Post](../resources/post.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae25e-132">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae25e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae25e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae25e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae25e-134">Request</span></span>
<span data-ttu-id="ae25e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae25e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="ae25e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae25e-136">Response</span></span>
<span data-ttu-id="ae25e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae25e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
            "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
            "id":"AQMkADgAAAIJbQAAAA==",
            "createdDateTime":"2018-01-11T17:36:17Z",
            "lastModifiedDateTime":"2018-01-11T17:36:17Z",
            "importance": "normal",
            "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
            "categories":[

            ],
            "receivedDateTime":"2018-01-11T17:36:17Z",
            "hasAttachments":false,
            "body":{
                "contentType":"html",
                "content":"<html><body></body></html>"
            },
            "from":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            },
            "sender":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            }
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
