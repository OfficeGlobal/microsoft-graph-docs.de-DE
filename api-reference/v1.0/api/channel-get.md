---
title: Abrufen von DDE-Kanal
description: Rufen Sie die Eigenschaften und die Beziehungen eines Kanals ab.
author: nkramer
ms.openlocfilehash: 38081fbc23e0f77dc69d1dbb6beba64b8f6d0a82
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324773"
---
# <a name="get-channel"></a><span data-ttu-id="8b693-103">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="8b693-103">Get channel</span></span>



<span data-ttu-id="8b693-104">Abrufen der Eigenschaften und die Beziehungen eines [DDE-Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8b693-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b693-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b693-105">Permissions</span></span>
<span data-ttu-id="8b693-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b693-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b693-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b693-108">Permission type</span></span>      | <span data-ttu-id="8b693-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b693-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b693-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b693-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b693-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b693-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b693-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b693-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b693-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b693-113">Not supported.</span></span>    |
|<span data-ttu-id="8b693-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b693-114">Application</span></span> | <span data-ttu-id="8b693-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b693-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8b693-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8b693-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8b693-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="8b693-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b693-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b693-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b693-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8b693-119">Optional query parameters</span></span>

<span data-ttu-id="8b693-120">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="8b693-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b693-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b693-121">Request headers</span></span>
| <span data-ttu-id="8b693-122">Header</span><span class="sxs-lookup"><span data-stu-id="8b693-122">Header</span></span>       | <span data-ttu-id="8b693-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8b693-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b693-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b693-124">Authorization</span></span>  | <span data-ttu-id="8b693-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b693-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b693-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b693-127">Request body</span></span>
<span data-ttu-id="8b693-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8b693-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b693-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b693-129">Response</span></span>

<span data-ttu-id="8b693-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Channel](../resources/channel.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b693-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b693-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b693-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b693-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b693-132">Request</span></span>
<span data-ttu-id="8b693-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b693-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="8b693-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b693-134">Response</span></span>
<span data-ttu-id="8b693-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b693-135">Here is an example of the response.</span></span> 

><span data-ttu-id="8b693-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8b693-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
