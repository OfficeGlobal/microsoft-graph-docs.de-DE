---
title: Beitrag abrufen
description: 'Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können das übergeordnete Element angeben. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8e724a664e708503daf5b30afdec04cccbb2fee4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912939"
---
# <a name="get-post"></a><span data-ttu-id="42698-104">Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="42698-104">Get post</span></span>

<span data-ttu-id="42698-p102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="42698-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="42698-107">Da die **post**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **post**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="42698-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="42698-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42698-108">Permissions</span></span>
<span data-ttu-id="42698-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42698-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42698-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42698-111">Permission type</span></span>      | <span data-ttu-id="42698-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42698-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42698-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42698-113">Delegated (work or school account)</span></span> | <span data-ttu-id="42698-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42698-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42698-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42698-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42698-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42698-116">Not supported.</span></span>    |
|<span data-ttu-id="42698-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42698-117">Application</span></span> | <span data-ttu-id="42698-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42698-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42698-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42698-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42698-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="42698-120">Optional query parameters</span></span>
<span data-ttu-id="42698-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="42698-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="42698-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42698-122">Request headers</span></span>
| <span data-ttu-id="42698-123">Header</span><span class="sxs-lookup"><span data-stu-id="42698-123">Header</span></span>       | <span data-ttu-id="42698-124">Wert</span><span class="sxs-lookup"><span data-stu-id="42698-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42698-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="42698-125">Authorization</span></span>  | <span data-ttu-id="42698-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42698-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42698-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42698-128">Request body</span></span>
<span data-ttu-id="42698-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="42698-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42698-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="42698-130">Response</span></span>

<span data-ttu-id="42698-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/post.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42698-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42698-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42698-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42698-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42698-133">Request</span></span>
<span data-ttu-id="42698-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42698-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="42698-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="42698-135">Response</span></span>
<span data-ttu-id="42698-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42698-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

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
  }
}
```

## <a name="see-also"></a><span data-ttu-id="42698-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="42698-139">See also</span></span>

- [<span data-ttu-id="42698-140">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="42698-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="42698-141">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="42698-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
