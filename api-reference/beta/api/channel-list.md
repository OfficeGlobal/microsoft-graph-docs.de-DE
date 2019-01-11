---
title: Liste Kanäle
description: Abrufen der Liste der Kanäle in dieser Gruppe.
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 23763e83f7e2e0d9333d39ebe439f8702b180f71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813524"
---
# <a name="list-channels"></a><span data-ttu-id="c52b6-103">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="c52b6-103">List channels</span></span>

> <span data-ttu-id="c52b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c52b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c52b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c52b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c52b6-106">Abrufen der Liste der [Kanäle](../resources/channel.md) in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c52b6-106">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="c52b6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c52b6-107">Permissions</span></span>
<span data-ttu-id="c52b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c52b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c52b6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c52b6-110">Permission type</span></span>      | <span data-ttu-id="c52b6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c52b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c52b6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c52b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c52b6-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c52b6-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c52b6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c52b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c52b6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c52b6-115">Not supported.</span></span>    |
|<span data-ttu-id="c52b6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c52b6-116">Application</span></span> | <span data-ttu-id="c52b6-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c52b6-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c52b6-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="c52b6-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c52b6-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="c52b6-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c52b6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c52b6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c52b6-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c52b6-121">Optional query parameters</span></span>
<span data-ttu-id="c52b6-122">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="c52b6-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c52b6-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c52b6-123">Request headers</span></span>
| <span data-ttu-id="c52b6-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c52b6-124">Header</span></span>       | <span data-ttu-id="c52b6-125">Wert</span><span class="sxs-lookup"><span data-stu-id="c52b6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c52b6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c52b6-126">Authorization</span></span>  | <span data-ttu-id="c52b6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c52b6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c52b6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c52b6-129">Request body</span></span>
<span data-ttu-id="c52b6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c52b6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c52b6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c52b6-131">Response</span></span>

<span data-ttu-id="c52b6-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DDE-Kanal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="c52b6-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c52b6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c52b6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c52b6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c52b6-134">Request</span></span>
<span data-ttu-id="c52b6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c52b6-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="c52b6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c52b6-136">Response</span></span>
<span data-ttu-id="c52b6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c52b6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
