---
title: Threads auflisten
description: Ruft alle Threads einer Gruppe ab.
ms.openlocfilehash: c805bfe2dac16b23311ebc58710525876cc3db9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059299"
---
# <a name="list-threads"></a><span data-ttu-id="d9f93-103">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="d9f93-103">List threads</span></span>

> <span data-ttu-id="d9f93-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d9f93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9f93-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9f93-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9f93-106">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="d9f93-106">Get all the threads of a group.</span></span>

<span data-ttu-id="d9f93-107">Hinweis: Sie können auch [Alle Threads einer Unterhaltung abrufen](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="d9f93-107">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9f93-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9f93-108">Permissions</span></span>
<span data-ttu-id="d9f93-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f93-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9f93-111">Permission type</span></span>      | <span data-ttu-id="d9f93-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9f93-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f93-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9f93-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9f93-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9f93-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9f93-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9f93-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f93-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9f93-116">Not supported.</span></span>    |
|<span data-ttu-id="d9f93-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9f93-117">Application</span></span> | <span data-ttu-id="d9f93-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9f93-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9f93-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9f93-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9f93-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d9f93-120">Optional query parameters</span></span>
<span data-ttu-id="d9f93-121">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9f93-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9f93-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9f93-122">Request headers</span></span>
| <span data-ttu-id="d9f93-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d9f93-123">Header</span></span>       | <span data-ttu-id="d9f93-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d9f93-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9f93-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9f93-125">Authorization</span></span>  | <span data-ttu-id="d9f93-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9f93-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9f93-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9f93-128">Request body</span></span>
<span data-ttu-id="d9f93-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9f93-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9f93-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9f93-130">Response</span></span>
<span data-ttu-id="d9f93-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversationThread](../resources/conversationthread.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9f93-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9f93-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9f93-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d9f93-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9f93-133">Request</span></span>
<span data-ttu-id="d9f93-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9f93-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="d9f93-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9f93-135">Response</span></span>
<span data-ttu-id="d9f93-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9f93-136">The following is an example of the response.</span></span>
><span data-ttu-id="d9f93-137">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d9f93-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d9f93-138">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d9f93-138">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
