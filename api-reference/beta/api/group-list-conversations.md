---
title: Unterhaltungen auflisten
description: Mit dieser API können Sie eine Liste aller Unterhaltungen in einer Gruppe abrufen.
author: dkershaw10
ms.openlocfilehash: 843ec498c577532fb8f74232314cbcbd3ec2569f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302667"
---
# <a name="list-conversations"></a><span data-ttu-id="be7a3-103">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="be7a3-103">List conversations</span></span>

> <span data-ttu-id="be7a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be7a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be7a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be7a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be7a3-106">Mit dieser API können Sie eine Liste aller [Unterhaltungen](../resources/conversation.md) in einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="be7a3-106">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="be7a3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be7a3-107">Permissions</span></span>
<span data-ttu-id="be7a3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be7a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be7a3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be7a3-110">Permission type</span></span>      | <span data-ttu-id="be7a3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be7a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be7a3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be7a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be7a3-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be7a3-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="be7a3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be7a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be7a3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be7a3-115">Not supported.</span></span>    |
|<span data-ttu-id="be7a3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be7a3-116">Application</span></span> | <span data-ttu-id="be7a3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be7a3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be7a3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be7a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be7a3-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be7a3-119">Optional query parameters</span></span>
<span data-ttu-id="be7a3-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be7a3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be7a3-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be7a3-121">Request headers</span></span>
| <span data-ttu-id="be7a3-122">Header</span><span class="sxs-lookup"><span data-stu-id="be7a3-122">Header</span></span>       | <span data-ttu-id="be7a3-123">Wert</span><span class="sxs-lookup"><span data-stu-id="be7a3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be7a3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be7a3-124">Authorization</span></span>  | <span data-ttu-id="be7a3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be7a3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be7a3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be7a3-127">Request body</span></span>
<span data-ttu-id="be7a3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be7a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be7a3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="be7a3-129">Response</span></span>
<span data-ttu-id="be7a3-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversation](../resources/conversation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be7a3-130">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be7a3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be7a3-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="be7a3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be7a3-132">Request</span></span>
<span data-ttu-id="be7a3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be7a3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="be7a3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="be7a3-134">Response</span></span>
<span data-ttu-id="be7a3-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be7a3-135">The following is an example of the response.</span></span>
><span data-ttu-id="be7a3-136">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="be7a3-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be7a3-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="be7a3-137">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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