---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste aller Objekte des Typs attachment abrufen, die einem Beitrag angefügt sind.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 910e269fb860ff21ecb80b8bcd247f9f9d43c947
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527012"
---
# <a name="list-attachments"></a><span data-ttu-id="ef618-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="ef618-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef618-104">Mit dieser API können Sie eine Liste aller Objekte des Typs [attachment](../resources/attachment.md) abrufen, die einem Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="ef618-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef618-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef618-105">Permissions</span></span>
<span data-ttu-id="ef618-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef618-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef618-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef618-108">Permission type</span></span>      | <span data-ttu-id="ef618-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef618-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef618-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef618-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef618-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef618-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef618-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef618-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef618-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef618-113">Not supported.</span></span>    |
|<span data-ttu-id="ef618-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef618-114">Application</span></span> | <span data-ttu-id="ef618-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef618-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef618-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef618-116">HTTP request</span></span>
<span data-ttu-id="ef618-117"><!-- { "blockType": "ignored" } -->Anlagen für einen [Posten](../resources/post.md) in einem [Thread](../resources/conversationthread.md) , die zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehören.</span><span class="sxs-lookup"><span data-stu-id="ef618-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef618-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ef618-118">Optional query parameters</span></span>
<span data-ttu-id="ef618-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef618-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ef618-120">Insbesondere können Sie die $ Abfragezeichenfolgen-Parameter, um alle der Post Anlagen Inline mit dem Rest der Post-Eigenschaften zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="ef618-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="ef618-121">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ef618-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="ef618-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef618-122">Request headers</span></span>
| <span data-ttu-id="ef618-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef618-123">Header</span></span>       | <span data-ttu-id="ef618-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ef618-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef618-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef618-125">Authorization</span></span>  | <span data-ttu-id="ef618-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef618-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef618-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef618-128">Request body</span></span>
<span data-ttu-id="ef618-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef618-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef618-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef618-130">Response</span></span>

<span data-ttu-id="ef618-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef618-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef618-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef618-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef618-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef618-133">Request</span></span>
<span data-ttu-id="ef618-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef618-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="ef618-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef618-135">Response</span></span>
<span data-ttu-id="ef618-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef618-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
