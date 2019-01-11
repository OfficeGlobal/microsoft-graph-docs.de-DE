---
title: Threads auflisten
description: Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: e1aacab39dfeae4dd9271ce5f3664c55eb80a583
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813307"
---
# <a name="list-threads"></a><span data-ttu-id="0758a-103">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="0758a-103">List threads</span></span>

> <span data-ttu-id="0758a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0758a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0758a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0758a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0758a-106">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="0758a-106">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="0758a-107">Hinweis: Sie können auch [Alle Threads einer Gruppe abrufen](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="0758a-107">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0758a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0758a-108">Permissions</span></span>
<span data-ttu-id="0758a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0758a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0758a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0758a-111">Permission type</span></span>      | <span data-ttu-id="0758a-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0758a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0758a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0758a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0758a-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0758a-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="0758a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0758a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0758a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0758a-116">Not supported.</span></span>    |
|<span data-ttu-id="0758a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0758a-117">Application</span></span> | <span data-ttu-id="0758a-118">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0758a-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0758a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0758a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0758a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0758a-120">Optional query parameters</span></span>
<span data-ttu-id="0758a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0758a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0758a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0758a-122">Request headers</span></span>
| <span data-ttu-id="0758a-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0758a-123">Header</span></span>       | <span data-ttu-id="0758a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="0758a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0758a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0758a-125">Authorization</span></span>  | <span data-ttu-id="0758a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0758a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0758a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0758a-128">Request body</span></span>
<span data-ttu-id="0758a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0758a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0758a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0758a-130">Response</span></span>

<span data-ttu-id="0758a-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversationThread](../resources/conversationthread.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0758a-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0758a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0758a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0758a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0758a-133">Request</span></span>
<span data-ttu-id="0758a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0758a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="0758a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0758a-135">Response</span></span>
<span data-ttu-id="0758a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0758a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
