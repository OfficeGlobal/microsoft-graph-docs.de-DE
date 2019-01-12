---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste aller Objekte des Typs attachment abrufen, die einem Beitrag angefügt sind.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 690b4ab540982dc9b7febcd1ea302afbcf8429ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916299"
---
# <a name="list-attachments"></a><span data-ttu-id="a511a-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="a511a-103">List attachments</span></span>

> <span data-ttu-id="a511a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a511a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a511a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a511a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a511a-106">Mit dieser API können Sie eine Liste aller Objekte des Typs [attachment](../resources/attachment.md) abrufen, die einem Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="a511a-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="a511a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a511a-107">Permissions</span></span>
<span data-ttu-id="a511a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a511a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a511a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a511a-110">Permission type</span></span>      | <span data-ttu-id="a511a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a511a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a511a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a511a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a511a-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a511a-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a511a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a511a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a511a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a511a-115">Not supported.</span></span>    |
|<span data-ttu-id="a511a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a511a-116">Application</span></span> | <span data-ttu-id="a511a-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a511a-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a511a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a511a-118">HTTP request</span></span>
<span data-ttu-id="a511a-119"><!-- { "blockType": "ignored" } -->Anlagen für einen [Posten](../resources/post.md) in einem [Thread](../resources/conversationthread.md) , die zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehören.</span><span class="sxs-lookup"><span data-stu-id="a511a-119"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a511a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a511a-120">Optional query parameters</span></span>
<span data-ttu-id="a511a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a511a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a511a-122">Insbesondere können Sie die $ Abfragezeichenfolgen-Parameter, um alle der Post Anlagen Inline mit dem Rest der Post-Eigenschaften zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="a511a-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="a511a-123">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="a511a-123">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="a511a-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a511a-124">Request headers</span></span>
| <span data-ttu-id="a511a-125">Header</span><span class="sxs-lookup"><span data-stu-id="a511a-125">Header</span></span>       | <span data-ttu-id="a511a-126">Wert</span><span class="sxs-lookup"><span data-stu-id="a511a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a511a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a511a-127">Authorization</span></span>  | <span data-ttu-id="a511a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a511a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a511a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a511a-130">Request body</span></span>
<span data-ttu-id="a511a-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a511a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a511a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a511a-132">Response</span></span>

<span data-ttu-id="a511a-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a511a-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a511a-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a511a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a511a-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a511a-135">Request</span></span>
<span data-ttu-id="a511a-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a511a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="a511a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="a511a-137">Response</span></span>
<span data-ttu-id="a511a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a511a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
