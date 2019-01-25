---
title: Threads auflisten
description: Ruft alle Threads einer Gruppe ab.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a4d0e0404828bda0aebe745d0b6413963d79a7ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520998"
---
# <a name="list-threads"></a><span data-ttu-id="8c3c5-103">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="8c3c5-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c3c5-104">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-104">Get all the threads of a group.</span></span>

<span data-ttu-id="8c3c5-105">Hinweis: Sie können auch [Alle Threads einer Unterhaltung abrufen](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="8c3c5-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c3c5-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8c3c5-106">Permissions</span></span>
<span data-ttu-id="8c3c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c3c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c3c5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c3c5-109">Permission type</span></span>      | <span data-ttu-id="8c3c5-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c3c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c3c5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c3c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c3c5-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c3c5-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c3c5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c3c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c3c5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c3c5-114">Not supported.</span></span>    |
|<span data-ttu-id="8c3c5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c3c5-115">Application</span></span> | <span data-ttu-id="8c3c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c3c5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c3c5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c3c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c3c5-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8c3c5-118">Optional query parameters</span></span>
<span data-ttu-id="8c3c5-119">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c3c5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c3c5-120">Request headers</span></span>
| <span data-ttu-id="8c3c5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8c3c5-121">Header</span></span>       | <span data-ttu-id="8c3c5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c3c5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c3c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c3c5-123">Authorization</span></span>  | <span data-ttu-id="8c3c5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c3c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c3c5-126">Request body</span></span>
<span data-ttu-id="8c3c5-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c3c5-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c3c5-128">Response</span></span>
<span data-ttu-id="8c3c5-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversationThread](../resources/conversationthread.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c3c5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c3c5-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8c3c5-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c3c5-131">Request</span></span>
<span data-ttu-id="8c3c5-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="8c3c5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c3c5-133">Response</span></span>
<span data-ttu-id="8c3c5-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-134">The following is an example of the response.</span></span>
><span data-ttu-id="8c3c5-135">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c3c5-136">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8c3c5-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
