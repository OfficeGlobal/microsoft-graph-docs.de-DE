---
title: conversationThread abrufen
description: 'Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f53afdd5416e2973c79ce3ec47e5101d3126d20f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510512"
---
# <a name="get-conversationthread"></a><span data-ttu-id="1499f-104">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="1499f-104">Get conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1499f-p102">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="1499f-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="1499f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1499f-107">Permissions</span></span>
<span data-ttu-id="1499f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1499f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1499f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1499f-110">Permission type</span></span>      | <span data-ttu-id="1499f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1499f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1499f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1499f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1499f-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1499f-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1499f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1499f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1499f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1499f-115">Not supported.</span></span>    |
|<span data-ttu-id="1499f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1499f-116">Application</span></span> | <span data-ttu-id="1499f-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1499f-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1499f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1499f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1499f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1499f-119">Optional query parameters</span></span>
<span data-ttu-id="1499f-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1499f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1499f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1499f-121">Request headers</span></span>
| <span data-ttu-id="1499f-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1499f-122">Header</span></span>       | <span data-ttu-id="1499f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="1499f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1499f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1499f-124">Authorization</span></span>  | <span data-ttu-id="1499f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1499f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1499f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1499f-127">Request body</span></span>
<span data-ttu-id="1499f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1499f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1499f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1499f-129">Response</span></span>

<span data-ttu-id="1499f-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1499f-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1499f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1499f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1499f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1499f-132">Request</span></span>
<span data-ttu-id="1499f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1499f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="1499f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1499f-134">Response</span></span>
<span data-ttu-id="1499f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1499f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
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
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
