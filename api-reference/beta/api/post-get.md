---
title: Beitrag abrufen
description: 'Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können das übergeordnete Element angeben. '
author: dkershaw10
ms.openlocfilehash: 98bed589c1982411f3c0b989e28e04d2e6166466
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361236"
---
# <a name="get-post"></a><span data-ttu-id="2722a-104">Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="2722a-104">Get post</span></span>

> <span data-ttu-id="2722a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2722a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2722a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2722a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2722a-p103">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="2722a-p103">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="2722a-109">Da die **post**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **post**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="2722a-109">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="2722a-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2722a-110">Permissions</span></span>
<span data-ttu-id="2722a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2722a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2722a-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2722a-113">Permission type</span></span>      | <span data-ttu-id="2722a-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2722a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2722a-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2722a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2722a-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2722a-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2722a-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2722a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2722a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2722a-118">Not supported.</span></span>    |
|<span data-ttu-id="2722a-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2722a-119">Application</span></span> | <span data-ttu-id="2722a-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2722a-120">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2722a-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2722a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2722a-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2722a-122">Optional query parameters</span></span>
<span data-ttu-id="2722a-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2722a-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2722a-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2722a-124">Request headers</span></span>
| <span data-ttu-id="2722a-125">Header</span><span class="sxs-lookup"><span data-stu-id="2722a-125">Header</span></span>       | <span data-ttu-id="2722a-126">Wert</span><span class="sxs-lookup"><span data-stu-id="2722a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2722a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2722a-127">Authorization</span></span>  | <span data-ttu-id="2722a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2722a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2722a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2722a-130">Request body</span></span>
<span data-ttu-id="2722a-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2722a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2722a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2722a-132">Response</span></span>

<span data-ttu-id="2722a-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/post.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2722a-133">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2722a-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2722a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2722a-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2722a-135">Request</span></span>
<span data-ttu-id="2722a-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2722a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="2722a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2722a-137">Response</span></span>
<span data-ttu-id="2722a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2722a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
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
```

## <a name="see-also"></a><span data-ttu-id="2722a-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2722a-141">See also</span></span>

- [<span data-ttu-id="2722a-142">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="2722a-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2722a-143">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="2722a-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2722a-144">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="2722a-144">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
