---
title: Unterhaltungen auflisten
description: Mit dieser API können Sie eine Liste aller Unterhaltungen in einer Gruppe abrufen.
author: dkershaw10
ms.openlocfilehash: 81b5b8deb9389d5aff6be9e537bb65ef43d366b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321399"
---
# <a name="list-conversations"></a><span data-ttu-id="8260d-103">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="8260d-103">List conversations</span></span>
<span data-ttu-id="8260d-104">Mit dieser API können Sie eine Liste aller [Unterhaltungen](../resources/conversation.md) in einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="8260d-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8260d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8260d-105">Permissions</span></span>
<span data-ttu-id="8260d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8260d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8260d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8260d-108">Permission type</span></span>      | <span data-ttu-id="8260d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8260d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8260d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8260d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8260d-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8260d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8260d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8260d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8260d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8260d-113">Not supported.</span></span>    |
|<span data-ttu-id="8260d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8260d-114">Application</span></span> | <span data-ttu-id="8260d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8260d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8260d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8260d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8260d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8260d-117">Optional query parameters</span></span>
<span data-ttu-id="8260d-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8260d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8260d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8260d-119">Request headers</span></span>
| <span data-ttu-id="8260d-120">Header</span><span class="sxs-lookup"><span data-stu-id="8260d-120">Header</span></span>       | <span data-ttu-id="8260d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8260d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8260d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8260d-122">Authorization</span></span>  | <span data-ttu-id="8260d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8260d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8260d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8260d-125">Request body</span></span>
<span data-ttu-id="8260d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8260d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8260d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="8260d-127">Response</span></span>
<span data-ttu-id="8260d-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversation](../resources/conversation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8260d-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8260d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8260d-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8260d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8260d-130">Request</span></span>
<span data-ttu-id="8260d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8260d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="8260d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8260d-132">Response</span></span>
<span data-ttu-id="8260d-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8260d-133">The following is an example of the response.</span></span>
><span data-ttu-id="8260d-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8260d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->