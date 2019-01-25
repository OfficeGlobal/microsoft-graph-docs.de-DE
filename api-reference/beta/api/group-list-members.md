---
title: Liste Gruppenmitglieder
description: Rufen Sie eine Liste der direkte Mitglieder der Gruppe. Eine Gruppe kann Benutzer, Kontakte, Geräte, Dienstprinzipale und anderen Gruppen als Mitglieder haben. Dieser Vorgang ist nicht transitiv.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f1643aa759926cd466d121d1c20ec1ae40bbc7cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509245"
---
# <a name="list-group-members"></a><span data-ttu-id="25fd0-105">Liste Gruppenmitglieder</span><span class="sxs-lookup"><span data-stu-id="25fd0-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25fd0-106">Rufen Sie eine Liste der direkte Mitglieder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="25fd0-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="25fd0-107">Eine Gruppe kann Benutzer, Kontakte, Geräte, Dienstprinzipale und anderen Gruppen als Mitglieder haben.</span><span class="sxs-lookup"><span data-stu-id="25fd0-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="25fd0-108">Dieser Vorgang ist nicht transitiv.</span><span class="sxs-lookup"><span data-stu-id="25fd0-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="25fd0-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25fd0-109">Permissions</span></span>

<span data-ttu-id="25fd0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25fd0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25fd0-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25fd0-112">Permission type</span></span>      | <span data-ttu-id="25fd0-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25fd0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25fd0-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25fd0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="25fd0-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="25fd0-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="25fd0-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25fd0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25fd0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25fd0-117">Not supported.</span></span>    |
|<span data-ttu-id="25fd0-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25fd0-118">Application</span></span> | <span data-ttu-id="25fd0-119">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="25fd0-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="25fd0-120">Hinweis: Um die Mitglieder einer Gruppe ausgeblendeten Mitgliedschaften aufzulisten, ist die Berechtigung Member.Read.Hidden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25fd0-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="25fd0-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25fd0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25fd0-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="25fd0-122">Optional query parameters</span></span>
<span data-ttu-id="25fd0-123">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="25fd0-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25fd0-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25fd0-124">Request headers</span></span>
| <span data-ttu-id="25fd0-125">Name</span><span class="sxs-lookup"><span data-stu-id="25fd0-125">Name</span></span>       | <span data-ttu-id="25fd0-126">Typ</span><span class="sxs-lookup"><span data-stu-id="25fd0-126">Type</span></span> | <span data-ttu-id="25fd0-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25fd0-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="25fd0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="25fd0-128">Authorization</span></span>  | <span data-ttu-id="25fd0-129">string</span><span class="sxs-lookup"><span data-stu-id="25fd0-129">string</span></span>  | <span data-ttu-id="25fd0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25fd0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25fd0-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25fd0-132">Request body</span></span>
<span data-ttu-id="25fd0-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="25fd0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25fd0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="25fd0-134">Response</span></span>
<span data-ttu-id="25fd0-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25fd0-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25fd0-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25fd0-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="25fd0-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25fd0-137">Request</span></span>
<span data-ttu-id="25fd0-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25fd0-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="25fd0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="25fd0-139">Response</span></span>
<span data-ttu-id="25fd0-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="25fd0-140">The following is an example of the response.</span></span>
><span data-ttu-id="25fd0-141">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="25fd0-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="25fd0-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="25fd0-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "@odata.type": "#microsoft.graph.user",
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
