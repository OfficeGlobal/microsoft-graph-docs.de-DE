---
title: Abrufen von DDE-Kanal
description: Rufen Sie die Eigenschaften und die Beziehungen eines Kanals ab.
ms.openlocfilehash: 977484c57d7d82d13b781f658bb53eea091e2066
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062788"
---
# <a name="get-channel"></a><span data-ttu-id="dfd60-103">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="dfd60-103">Get channel</span></span>

> <span data-ttu-id="dfd60-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dfd60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfd60-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dfd60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfd60-106">Abrufen der Eigenschaften und die Beziehungen eines [DDE-Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="dfd60-106">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfd60-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dfd60-107">Permissions</span></span>
<span data-ttu-id="dfd60-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfd60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd60-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dfd60-110">Permission type</span></span>      | <span data-ttu-id="dfd60-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dfd60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfd60-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dfd60-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dfd60-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd60-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfd60-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dfd60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfd60-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dfd60-115">Not supported.</span></span>    |
|<span data-ttu-id="dfd60-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dfd60-116">Application</span></span> | <span data-ttu-id="dfd60-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd60-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="dfd60-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfd60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfd60-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dfd60-119">Optional query parameters</span></span>

<span data-ttu-id="dfd60-120">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="dfd60-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfd60-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dfd60-121">Request headers</span></span>
| <span data-ttu-id="dfd60-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dfd60-122">Header</span></span>       | <span data-ttu-id="dfd60-123">Wert</span><span class="sxs-lookup"><span data-stu-id="dfd60-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfd60-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfd60-124">Authorization</span></span>  | <span data-ttu-id="dfd60-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dfd60-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfd60-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dfd60-127">Request body</span></span>
<span data-ttu-id="dfd60-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dfd60-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfd60-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfd60-129">Response</span></span>

<span data-ttu-id="dfd60-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Channel](../resources/channel.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dfd60-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfd60-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dfd60-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfd60-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfd60-132">Request</span></span>
<span data-ttu-id="dfd60-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dfd60-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="dfd60-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfd60-134">Response</span></span>
<span data-ttu-id="dfd60-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dfd60-135">Here is an example of the response.</span></span> 

><span data-ttu-id="dfd60-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="dfd60-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
