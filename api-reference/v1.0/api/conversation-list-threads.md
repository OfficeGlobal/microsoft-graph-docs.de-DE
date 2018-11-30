---
title: Threads auflisten
description: Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.
ms.openlocfilehash: 9d3a981b71b369e745acae0b362e5711a18f0272
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018523"
---
# <a name="list-threads"></a><span data-ttu-id="f035e-103">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="f035e-103">List threads</span></span>

<span data-ttu-id="f035e-104">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="f035e-104">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="f035e-105">Hinweis: Sie können auch [Alle Threads einer Gruppe abrufen](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="f035e-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f035e-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f035e-106">Permissions</span></span>
<span data-ttu-id="f035e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f035e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f035e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f035e-109">Permission type</span></span>      | <span data-ttu-id="f035e-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f035e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f035e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f035e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f035e-112">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f035e-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="f035e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f035e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f035e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f035e-114">Not supported.</span></span>    |
|<span data-ttu-id="f035e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f035e-115">Application</span></span> | <span data-ttu-id="f035e-116">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f035e-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f035e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f035e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f035e-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f035e-118">Optional query parameters</span></span>
<span data-ttu-id="f035e-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f035e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f035e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f035e-120">Request headers</span></span>
| <span data-ttu-id="f035e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f035e-121">Header</span></span>       | <span data-ttu-id="f035e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f035e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f035e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f035e-123">Authorization</span></span>  | <span data-ttu-id="f035e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f035e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f035e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f035e-126">Request body</span></span>
<span data-ttu-id="f035e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f035e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f035e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f035e-128">Response</span></span>

<span data-ttu-id="f035e-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversationThread](../resources/conversationthread.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f035e-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f035e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f035e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f035e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f035e-131">Request</span></span>
<span data-ttu-id="f035e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f035e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="f035e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f035e-133">Response</span></span>
<span data-ttu-id="f035e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f035e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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