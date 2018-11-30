---
title: Liste Kanäle
description: Abrufen der Liste der Kanäle in dieser Gruppe.
ms.openlocfilehash: 5f96d4c47a787839626a9d90733d087906407b01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017472"
---
# <a name="list-channels"></a><span data-ttu-id="bb62d-103">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="bb62d-103">List channels</span></span>



<span data-ttu-id="bb62d-104">Abrufen der Liste der [Kanäle](../resources/channel.md) in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="bb62d-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb62d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb62d-105">Permissions</span></span>
<span data-ttu-id="bb62d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb62d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bb62d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb62d-108">Permission type</span></span>      | <span data-ttu-id="bb62d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb62d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb62d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb62d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb62d-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb62d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb62d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb62d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb62d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb62d-113">Not supported.</span></span>    |
|<span data-ttu-id="bb62d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb62d-114">Application</span></span> | <span data-ttu-id="bb62d-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb62d-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="bb62d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb62d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb62d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bb62d-117">Optional query parameters</span></span>
<span data-ttu-id="bb62d-118">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="bb62d-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb62d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb62d-119">Request headers</span></span>
| <span data-ttu-id="bb62d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bb62d-120">Header</span></span>       | <span data-ttu-id="bb62d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bb62d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb62d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb62d-122">Authorization</span></span>  | <span data-ttu-id="bb62d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb62d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb62d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb62d-125">Request body</span></span>
<span data-ttu-id="bb62d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb62d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb62d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb62d-127">Response</span></span>

<span data-ttu-id="bb62d-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DDE-Kanal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="bb62d-128">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb62d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb62d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb62d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb62d-130">Request</span></span>
<span data-ttu-id="bb62d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb62d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="bb62d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb62d-132">Response</span></span>
<span data-ttu-id="bb62d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb62d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
