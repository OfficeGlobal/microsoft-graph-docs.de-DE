---
title: Liste Kanäle
description: Abrufen der Liste der Kanäle in dieser Gruppe.
ms.openlocfilehash: af97bbcd127c413ac11fcc0a8e40784a6c58b593
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222625"
---
# <a name="list-channels"></a><span data-ttu-id="290aa-103">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="290aa-103">List channels</span></span>



<span data-ttu-id="290aa-104">Abrufen der Liste der [Kanäle](../resources/channel.md) in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="290aa-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="290aa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="290aa-105">Permissions</span></span>
<span data-ttu-id="290aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="290aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="290aa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="290aa-108">Permission type</span></span>      | <span data-ttu-id="290aa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="290aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="290aa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="290aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="290aa-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="290aa-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="290aa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="290aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="290aa-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="290aa-113">Not supported.</span></span>    |
|<span data-ttu-id="290aa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="290aa-114">Application</span></span> | <span data-ttu-id="290aa-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="290aa-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="290aa-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="290aa-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="290aa-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="290aa-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="290aa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="290aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="290aa-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="290aa-119">Optional query parameters</span></span>
<span data-ttu-id="290aa-120">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="290aa-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="290aa-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="290aa-121">Request headers</span></span>
| <span data-ttu-id="290aa-122">Header</span><span class="sxs-lookup"><span data-stu-id="290aa-122">Header</span></span>       | <span data-ttu-id="290aa-123">Wert</span><span class="sxs-lookup"><span data-stu-id="290aa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="290aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="290aa-124">Authorization</span></span>  | <span data-ttu-id="290aa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="290aa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="290aa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="290aa-127">Request body</span></span>
<span data-ttu-id="290aa-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="290aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="290aa-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="290aa-129">Response</span></span>

<span data-ttu-id="290aa-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DDE-Kanal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="290aa-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="290aa-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="290aa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="290aa-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="290aa-132">Request</span></span>
<span data-ttu-id="290aa-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="290aa-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="290aa-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="290aa-134">Response</span></span>
<span data-ttu-id="290aa-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="290aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
