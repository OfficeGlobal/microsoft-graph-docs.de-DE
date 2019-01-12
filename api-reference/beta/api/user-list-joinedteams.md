---
title: joinedTeams auflisten
description: Abrufen des Teams für die der Microsoft-Teams, die der Benutzer ein direktes Mitglied ist.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 839b6531318ca9fc8abb3fd3544566622d02a78b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938202"
---
# <a name="list-joinedteams"></a><span data-ttu-id="5780d-103">joinedTeams auflisten</span><span class="sxs-lookup"><span data-stu-id="5780d-103">List joinedTeams</span></span>

> <span data-ttu-id="5780d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5780d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5780d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5780d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5780d-106">Rufen Sie die [Teams](../resources/team.md) in Microsoft-Teams, die der Benutzer ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="5780d-106">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="5780d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5780d-107">Permissions</span></span>
<span data-ttu-id="5780d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5780d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5780d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5780d-110">Permission type</span></span>      | <span data-ttu-id="5780d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5780d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5780d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5780d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5780d-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5780d-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="5780d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5780d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5780d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5780d-115">Not supported.</span></span>    |
|<span data-ttu-id="5780d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5780d-116">Application</span></span> | <span data-ttu-id="5780d-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5780d-117">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="5780d-118">Derzeit arbeitet mit Berechtigungen delegiert wurde dieser Vorgang nur für "me" Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5780d-118">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="5780d-119">Bei den Anwendungsberechtigungen funktioniert dies für alle Benutzer durch bestimmte Benutzer-Id angeben. ("me" ist alias nicht mit den Anwendungsberechtigungen unterstützt) Weitere Informationen hierzu finden Sie unter [bekannte Probleme](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span><span class="sxs-lookup"><span data-stu-id="5780d-119">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="5780d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5780d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5780d-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5780d-121">Optional query parameters</span></span>
<span data-ttu-id="5780d-122">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5780d-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5780d-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5780d-123">Request headers</span></span>
| <span data-ttu-id="5780d-124">Header</span><span class="sxs-lookup"><span data-stu-id="5780d-124">Header</span></span>       | <span data-ttu-id="5780d-125">Wert</span><span class="sxs-lookup"><span data-stu-id="5780d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5780d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5780d-126">Authorization</span></span>  | <span data-ttu-id="5780d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5780d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5780d-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5780d-129">Accept</span></span>  | <span data-ttu-id="5780d-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5780d-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5780d-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5780d-131">Request body</span></span>
<span data-ttu-id="5780d-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5780d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5780d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5780d-133">Response</span></span>

<span data-ttu-id="5780d-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5780d-134">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5780d-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5780d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5780d-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5780d-136">Request</span></span>
<span data-ttu-id="5780d-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5780d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="5780d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5780d-138">Response</span></span>
<span data-ttu-id="5780d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5780d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="5780d-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5780d-142">See also</span></span>
[<span data-ttu-id="5780d-143">Listen Sie alle teams</span><span class="sxs-lookup"><span data-stu-id="5780d-143">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
