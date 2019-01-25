---
title: Beiträge auflisten
description: 'Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6ab9658753baceed8b983eb493957503179f5865
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517246"
---
# <a name="list-posts"></a><span data-ttu-id="f5a2e-104">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="f5a2e-104">List posts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5a2e-p102">Dient zum Abrufen der Beiträge des angegebenen Threads. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5a2e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5a2e-107">Permissions</span></span>
<span data-ttu-id="f5a2e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5a2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5a2e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5a2e-110">Permission type</span></span>      | <span data-ttu-id="f5a2e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5a2e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5a2e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5a2e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5a2e-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5a2e-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="f5a2e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5a2e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5a2e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5a2e-115">Not supported.</span></span>    |
|<span data-ttu-id="f5a2e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5a2e-116">Application</span></span> | <span data-ttu-id="f5a2e-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5a2e-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5a2e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5a2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5a2e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f5a2e-119">Optional query parameters</span></span>
<span data-ttu-id="f5a2e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5a2e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5a2e-121">Request headers</span></span>
| <span data-ttu-id="f5a2e-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f5a2e-122">Header</span></span>       | <span data-ttu-id="f5a2e-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f5a2e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5a2e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5a2e-124">Authorization</span></span>  | <span data-ttu-id="f5a2e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5a2e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5a2e-127">Request body</span></span>
<span data-ttu-id="f5a2e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5a2e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5a2e-129">Response</span></span>

<span data-ttu-id="f5a2e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Post](../resources/post.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5a2e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5a2e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5a2e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5a2e-132">Request</span></span>
<span data-ttu-id="f5a2e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="f5a2e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5a2e-134">Response</span></span>
<span data-ttu-id="f5a2e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5a2e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-list-posts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
