---
title: Unterhaltung abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Unterhaltungsobjekts abrufen.
author: dkershaw10
ms.openlocfilehash: 7f5beb49140c898a4afeb059402c06fdade5f7ba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333950"
---
# <a name="get-conversation"></a><span data-ttu-id="502ef-103">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="502ef-103">Get conversation</span></span>

> <span data-ttu-id="502ef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="502ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="502ef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="502ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="502ef-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Unterhaltungsobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="502ef-106">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="502ef-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="502ef-107">Permissions</span></span>
<span data-ttu-id="502ef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="502ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="502ef-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="502ef-110">Permission type</span></span>      | <span data-ttu-id="502ef-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="502ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="502ef-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="502ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="502ef-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="502ef-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="502ef-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="502ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="502ef-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="502ef-115">Not supported.</span></span>    |
|<span data-ttu-id="502ef-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="502ef-116">Application</span></span> | <span data-ttu-id="502ef-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="502ef-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="502ef-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="502ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="502ef-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="502ef-119">Optional query parameters</span></span>
<span data-ttu-id="502ef-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="502ef-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="502ef-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="502ef-121">Request headers</span></span>
| <span data-ttu-id="502ef-122">Header</span><span class="sxs-lookup"><span data-stu-id="502ef-122">Header</span></span>       | <span data-ttu-id="502ef-123">Wert</span><span class="sxs-lookup"><span data-stu-id="502ef-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="502ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="502ef-124">Authorization</span></span>  | <span data-ttu-id="502ef-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="502ef-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="502ef-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="502ef-127">Request body</span></span>
<span data-ttu-id="502ef-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="502ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="502ef-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="502ef-129">Response</span></span>

<span data-ttu-id="502ef-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="502ef-130">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="502ef-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="502ef-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="502ef-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="502ef-132">Request</span></span>
<span data-ttu-id="502ef-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="502ef-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="502ef-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="502ef-134">Response</span></span>
<span data-ttu-id="502ef-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="502ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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
