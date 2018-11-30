---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste aller Objekte des Typs attachment abrufen, die einem Beitrag angefügt sind.
ms.openlocfilehash: b1a7ea8778b2ff25ad8e3159697d12aafe180506
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019985"
---
# <a name="list-attachments"></a><span data-ttu-id="fbde7-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="fbde7-103">List attachments</span></span>

<span data-ttu-id="fbde7-104">Mit dieser API können Sie eine Liste aller Objekte des Typs [attachment](../resources/attachment.md) abrufen, die einem Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="fbde7-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="fbde7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fbde7-105">Permissions</span></span>
<span data-ttu-id="fbde7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbde7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbde7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbde7-108">Permission type</span></span>      | <span data-ttu-id="fbde7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbde7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbde7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbde7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fbde7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbde7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbde7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbde7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbde7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbde7-113">Not supported.</span></span>    |
|<span data-ttu-id="fbde7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbde7-114">Application</span></span> | <span data-ttu-id="fbde7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbde7-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbde7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbde7-116">HTTP request</span></span>
<span data-ttu-id="fbde7-117"><!-- { "blockType": "ignored" } -->Anlagen für einen [Posten](../resources/post.md) in einem [Thread](../resources/conversationthread.md) , die zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehören.</span><span class="sxs-lookup"><span data-stu-id="fbde7-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fbde7-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fbde7-118">Optional query parameters</span></span>
<span data-ttu-id="fbde7-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fbde7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fbde7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbde7-120">Request headers</span></span>
| <span data-ttu-id="fbde7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fbde7-121">Header</span></span>       | <span data-ttu-id="fbde7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fbde7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbde7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbde7-123">Authorization</span></span>  | <span data-ttu-id="fbde7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fbde7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbde7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbde7-126">Request body</span></span>
<span data-ttu-id="fbde7-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fbde7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbde7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbde7-128">Response</span></span>

<span data-ttu-id="fbde7-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbde7-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbde7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbde7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbde7-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbde7-131">Request</span></span>
<span data-ttu-id="fbde7-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbde7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="fbde7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbde7-133">Response</span></span>
<span data-ttu-id="fbde7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbde7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
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
