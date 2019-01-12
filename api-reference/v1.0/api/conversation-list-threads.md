---
title: Threads auflisten
description: Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3aefbf3dffd3c9aeb4244684316aec64a2c8f02b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917755"
---
# <a name="list-threads"></a><span data-ttu-id="bcf64-103">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="bcf64-103">List threads</span></span>

<span data-ttu-id="bcf64-104">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="bcf64-104">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="bcf64-105">Hinweis: Sie können auch [Alle Threads einer Gruppe abrufen](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="bcf64-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bcf64-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bcf64-106">Permissions</span></span>
<span data-ttu-id="bcf64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf64-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bcf64-109">Permission type</span></span>      | <span data-ttu-id="bcf64-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bcf64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcf64-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bcf64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bcf64-112">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcf64-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="bcf64-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bcf64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcf64-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcf64-114">Not supported.</span></span>    |
|<span data-ttu-id="bcf64-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bcf64-115">Application</span></span> | <span data-ttu-id="bcf64-116">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcf64-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcf64-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcf64-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bcf64-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bcf64-118">Optional query parameters</span></span>
<span data-ttu-id="bcf64-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bcf64-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bcf64-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bcf64-120">Request headers</span></span>
| <span data-ttu-id="bcf64-121">Header</span><span class="sxs-lookup"><span data-stu-id="bcf64-121">Header</span></span>       | <span data-ttu-id="bcf64-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bcf64-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcf64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcf64-123">Authorization</span></span>  | <span data-ttu-id="bcf64-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bcf64-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcf64-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bcf64-126">Request body</span></span>
<span data-ttu-id="bcf64-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bcf64-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcf64-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcf64-128">Response</span></span>

<span data-ttu-id="bcf64-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversationThread](../resources/conversationthread.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcf64-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bcf64-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bcf64-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcf64-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcf64-131">Request</span></span>
<span data-ttu-id="bcf64-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bcf64-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="bcf64-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcf64-133">Response</span></span>
<span data-ttu-id="bcf64-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcf64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "datetime-value",
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
