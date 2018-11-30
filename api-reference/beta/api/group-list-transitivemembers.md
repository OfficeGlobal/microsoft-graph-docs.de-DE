---
title: Transitive Gruppenmitglieder Liste
description: Rufen Sie eine Liste der Mitglieder der Gruppe. Eine Gruppe kann Benutzer, Kontakte, Geräte, Dienstprinzipale und anderen Gruppen als Mitglieder haben. Dieser Vorgang ist transitiv und gibt eine Liste aller geschachtelten Elemente ebenfalls zurück.
ms.openlocfilehash: a3cdc0048db3b3d1aa90b5d3426d22439a18b298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061530"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="fd157-105">Transitive Gruppenmitglieder Liste</span><span class="sxs-lookup"><span data-stu-id="fd157-105">List group transitive members</span></span>

> <span data-ttu-id="fd157-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd157-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd157-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd157-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd157-108">Rufen Sie eine Liste der Mitglieder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="fd157-108">Get a list of the group's members.</span></span> <span data-ttu-id="fd157-109">Eine Gruppe kann Benutzer, Kontakte, Geräte, Dienstprinzipale und anderen Gruppen als Mitglieder haben.</span><span class="sxs-lookup"><span data-stu-id="fd157-109">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="fd157-110">Dieser Vorgang ist transitiv und gibt eine Liste aller geschachtelten Elemente ebenfalls zurück.</span><span class="sxs-lookup"><span data-stu-id="fd157-110">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd157-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd157-111">Permissions</span></span>

<span data-ttu-id="fd157-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd157-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd157-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd157-114">Permission type</span></span>      | <span data-ttu-id="fd157-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd157-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd157-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd157-116">Delegated (work or school account)</span></span> | <span data-ttu-id="fd157-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd157-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="fd157-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd157-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd157-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd157-119">Not supported.</span></span>    |
|<span data-ttu-id="fd157-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd157-120">Application</span></span> | <span data-ttu-id="fd157-121">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd157-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="fd157-122">Hinweis: Um die Mitglieder einer Gruppe ausgeblendeten Mitgliedschaften aufzulisten, ist die Berechtigung Member.Read.Hidden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd157-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd157-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd157-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd157-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd157-124">Optional query parameters</span></span>

<span data-ttu-id="fd157-125">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd157-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd157-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd157-126">Request headers</span></span>

| <span data-ttu-id="fd157-127">Name</span><span class="sxs-lookup"><span data-stu-id="fd157-127">Name</span></span>       | <span data-ttu-id="fd157-128">Typ</span><span class="sxs-lookup"><span data-stu-id="fd157-128">Type</span></span> | <span data-ttu-id="fd157-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd157-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd157-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd157-130">Authorization</span></span>  | <span data-ttu-id="fd157-131">string</span><span class="sxs-lookup"><span data-stu-id="fd157-131">string</span></span>  | <span data-ttu-id="fd157-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd157-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd157-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd157-134">Request body</span></span>

<span data-ttu-id="fd157-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd157-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd157-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd157-136">Response</span></span>

<span data-ttu-id="fd157-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd157-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd157-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd157-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd157-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd157-139">Request</span></span>

<span data-ttu-id="fd157-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd157-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/tranisitiveMembers
```

### <a name="response"></a><span data-ttu-id="fd157-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd157-141">Response</span></span>

<span data-ttu-id="fd157-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd157-142">The following is an example of the response.</span></span>
><span data-ttu-id="fd157-143">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="fd157-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fd157-144">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fd157-144">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->