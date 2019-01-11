---
title: conversationThread abrufen
description: 'Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können angeben, der übergeordnete Unterhaltung und der Thread oder, '
localization_priority: Normal
ms.openlocfilehash: 61ec38651274cf71e87f362927de66873a6cca24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894243"
---
# <a name="get-conversationthread"></a><span data-ttu-id="d9681-104">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="d9681-104">Get conversationThread</span></span>

<span data-ttu-id="d9681-p102">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="d9681-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="d9681-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9681-107">Permissions</span></span>
<span data-ttu-id="d9681-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9681-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9681-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9681-110">Permission type</span></span>      | <span data-ttu-id="d9681-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9681-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9681-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9681-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9681-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9681-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="d9681-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9681-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9681-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9681-115">Not supported.</span></span>    |
|<span data-ttu-id="d9681-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9681-116">Application</span></span> | <span data-ttu-id="d9681-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9681-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9681-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9681-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9681-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d9681-119">Optional query parameters</span></span>
<span data-ttu-id="d9681-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9681-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9681-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9681-121">Request headers</span></span>
| <span data-ttu-id="d9681-122">Header</span><span class="sxs-lookup"><span data-stu-id="d9681-122">Header</span></span>       | <span data-ttu-id="d9681-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d9681-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9681-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9681-124">Authorization</span></span>  | <span data-ttu-id="d9681-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9681-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9681-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9681-127">Request body</span></span>
<span data-ttu-id="d9681-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9681-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9681-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9681-129">Response</span></span>

<span data-ttu-id="d9681-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9681-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9681-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9681-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9681-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9681-132">Request</span></span>
<span data-ttu-id="d9681-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9681-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="d9681-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9681-134">Response</span></span>
<span data-ttu-id="d9681-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9681-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
