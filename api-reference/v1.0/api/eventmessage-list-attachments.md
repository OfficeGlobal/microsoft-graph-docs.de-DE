---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste von Anlagenobjekten abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 138759ad46af5ee5050e0c8e625d81e893c69725
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976716"
---
# <a name="list-attachments"></a><span data-ttu-id="088b4-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="088b4-103">List attachments</span></span>

<span data-ttu-id="088b4-104">Mit dieser API können Sie eine Liste von Anlagenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="088b4-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="088b4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="088b4-105">Permissions</span></span>
<span data-ttu-id="088b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="088b4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="088b4-108">Permission type</span></span>      | <span data-ttu-id="088b4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="088b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="088b4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="088b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="088b4-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="088b4-111">Mail.Read</span></span>    |
|<span data-ttu-id="088b4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="088b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="088b4-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="088b4-113">Mail.Read</span></span>    |
|<span data-ttu-id="088b4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="088b4-114">Application</span></span> | <span data-ttu-id="088b4-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="088b4-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="088b4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="088b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="088b4-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="088b4-117">Optional query parameters</span></span>
<span data-ttu-id="088b4-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="088b4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="088b4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="088b4-119">Request headers</span></span>
| <span data-ttu-id="088b4-120">Name</span><span class="sxs-lookup"><span data-stu-id="088b4-120">Name</span></span>       | <span data-ttu-id="088b4-121">Typ</span><span class="sxs-lookup"><span data-stu-id="088b4-121">Type</span></span> | <span data-ttu-id="088b4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="088b4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="088b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="088b4-123">Authorization</span></span>  | <span data-ttu-id="088b4-124">string</span><span class="sxs-lookup"><span data-stu-id="088b4-124">string</span></span>  | <span data-ttu-id="088b4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="088b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="088b4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="088b4-127">Request body</span></span>
<span data-ttu-id="088b4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="088b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="088b4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="088b4-129">Response</span></span>

<span data-ttu-id="088b4-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="088b4-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="088b4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="088b4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="088b4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="088b4-132">Request</span></span>
<span data-ttu-id="088b4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="088b4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="088b4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="088b4-134">Response</span></span>
<span data-ttu-id="088b4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="088b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
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
