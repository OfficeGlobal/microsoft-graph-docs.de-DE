---
title: joinedTeams auflisten
description: Abrufen des Teams für die der Microsoft-Teams, die der Benutzer ein direktes Mitglied ist.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 95dfa387a55dd5270035816d144ac3a6ac2b6703
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016702"
---
# <a name="list-joinedteams"></a><span data-ttu-id="e3f2f-103">joinedTeams auflisten</span><span class="sxs-lookup"><span data-stu-id="e3f2f-103">List joinedTeams</span></span>



<span data-ttu-id="e3f2f-104">Rufen Sie die [Teams](../resources/team.md) in Microsoft-Teams, die der Benutzer ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="e3f2f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3f2f-105">Permissions</span></span>
<span data-ttu-id="e3f2f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3f2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3f2f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3f2f-108">Permission type</span></span>      | <span data-ttu-id="e3f2f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3f2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3f2f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3f2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3f2f-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f2f-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3f2f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3f2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3f2f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3f2f-113">Not supported.</span></span>    |
|<span data-ttu-id="e3f2f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3f2f-114">Application</span></span> | <span data-ttu-id="e3f2f-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f2f-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="e3f2f-116">Mit delegiert Benutzerberechtigungen funktioniert diese Operation nur für "me" Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="e3f2f-117">Bei den Anwendungsberechtigungen funktioniert dies für alle Benutzer durch bestimmte Benutzer-Id angeben. ("me" ist alias nicht mit den Anwendungsberechtigungen unterstützt)</span><span class="sxs-lookup"><span data-stu-id="e3f2f-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="e3f2f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3f2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3f2f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e3f2f-119">Optional query parameters</span></span>
<span data-ttu-id="e3f2f-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3f2f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3f2f-121">Request headers</span></span>
| <span data-ttu-id="e3f2f-122">Header</span><span class="sxs-lookup"><span data-stu-id="e3f2f-122">Header</span></span>       | <span data-ttu-id="e3f2f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e3f2f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3f2f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3f2f-124">Authorization</span></span>  | <span data-ttu-id="e3f2f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3f2f-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3f2f-127">Accept</span></span>  | <span data-ttu-id="e3f2f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e3f2f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3f2f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3f2f-129">Request body</span></span>
<span data-ttu-id="e3f2f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3f2f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3f2f-131">Response</span></span>

<span data-ttu-id="e3f2f-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3f2f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3f2f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3f2f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3f2f-134">Request</span></span>
<span data-ttu-id="e3f2f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="e3f2f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3f2f-136">Response</span></span>
<span data-ttu-id="e3f2f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3f2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e3f2f-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e3f2f-140">See also</span></span>
[<span data-ttu-id="e3f2f-141">Listen Sie alle teams</span><span class="sxs-lookup"><span data-stu-id="e3f2f-141">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
