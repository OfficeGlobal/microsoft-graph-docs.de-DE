---
title: Unterhaltung abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Unterhaltungsobjekts abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 174d5a5b5309348de5ebf01d38445d032d9e31ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980391"
---
# <a name="get-conversation"></a><span data-ttu-id="29bcf-103">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="29bcf-103">Get conversation</span></span>

<span data-ttu-id="29bcf-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Unterhaltungsobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="29bcf-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="29bcf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29bcf-105">Permissions</span></span>
<span data-ttu-id="29bcf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29bcf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29bcf-108">Permission type</span></span>      | <span data-ttu-id="29bcf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29bcf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29bcf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29bcf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29bcf-111">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="29bcf-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="29bcf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29bcf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29bcf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29bcf-113">Not supported.</span></span>    |
|<span data-ttu-id="29bcf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29bcf-114">Application</span></span> | <span data-ttu-id="29bcf-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="29bcf-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29bcf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29bcf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="29bcf-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="29bcf-117">Optional query parameters</span></span>
<span data-ttu-id="29bcf-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29bcf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29bcf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29bcf-119">Request headers</span></span>
| <span data-ttu-id="29bcf-120">Header</span><span class="sxs-lookup"><span data-stu-id="29bcf-120">Header</span></span>       | <span data-ttu-id="29bcf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="29bcf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29bcf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29bcf-122">Authorization</span></span>  | <span data-ttu-id="29bcf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29bcf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29bcf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29bcf-125">Request body</span></span>
<span data-ttu-id="29bcf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29bcf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29bcf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="29bcf-127">Response</span></span>

<span data-ttu-id="29bcf-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29bcf-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29bcf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29bcf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29bcf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29bcf-130">Request</span></span>
<span data-ttu-id="29bcf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29bcf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="29bcf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="29bcf-132">Response</span></span>
<span data-ttu-id="29bcf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29bcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
