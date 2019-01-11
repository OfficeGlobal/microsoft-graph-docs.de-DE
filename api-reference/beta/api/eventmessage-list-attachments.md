---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste von Anlagenobjekten abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: b5ca42a0ee191b62ab8c5484acce41acf7d924a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853949"
---
# <a name="list-attachments"></a><span data-ttu-id="96ec6-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="96ec6-103">List attachments</span></span>

> <span data-ttu-id="96ec6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96ec6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96ec6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96ec6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96ec6-106">Mit dieser API können Sie eine Liste von Anlagenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="96ec6-106">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="96ec6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96ec6-107">Permissions</span></span>
<span data-ttu-id="96ec6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96ec6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ec6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96ec6-110">Permission type</span></span>      | <span data-ttu-id="96ec6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96ec6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96ec6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96ec6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96ec6-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96ec6-113">Mail.Read</span></span>    |
|<span data-ttu-id="96ec6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96ec6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96ec6-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96ec6-115">Mail.Read</span></span>    |
|<span data-ttu-id="96ec6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96ec6-116">Application</span></span> | <span data-ttu-id="96ec6-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96ec6-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="96ec6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96ec6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96ec6-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="96ec6-119">Optional query parameters</span></span>
<span data-ttu-id="96ec6-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96ec6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96ec6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96ec6-121">Request headers</span></span>
| <span data-ttu-id="96ec6-122">Name</span><span class="sxs-lookup"><span data-stu-id="96ec6-122">Name</span></span>       | <span data-ttu-id="96ec6-123">Typ</span><span class="sxs-lookup"><span data-stu-id="96ec6-123">Type</span></span> | <span data-ttu-id="96ec6-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96ec6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96ec6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96ec6-125">Authorization</span></span>  | <span data-ttu-id="96ec6-126">string</span><span class="sxs-lookup"><span data-stu-id="96ec6-126">string</span></span>  | <span data-ttu-id="96ec6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96ec6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96ec6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96ec6-129">Request body</span></span>
<span data-ttu-id="96ec6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="96ec6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96ec6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="96ec6-131">Response</span></span>

<span data-ttu-id="96ec6-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96ec6-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96ec6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96ec6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96ec6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96ec6-134">Request</span></span>
<span data-ttu-id="96ec6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96ec6-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="96ec6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="96ec6-136">Response</span></span>
<span data-ttu-id="96ec6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96ec6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
