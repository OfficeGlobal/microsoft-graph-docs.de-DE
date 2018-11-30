---
title: Liste Benutzer transitive Mitglied
description: Abrufen von Gruppen, Directory Rollen und administrative Einheiten, denen der Benutzer Mitglied ist. Diese API-Anforderung ist transitiv und alle Gruppen, die, denen der Benutzer ein geschachtelte Mitglied ist, wird ebenfalls zurückgegeben.
ms.openlocfilehash: b507e7e0e54fcd37b4a31a9a6cf9e07b32e41244
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065278"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="e4e83-104">Liste Benutzer transitive Mitglied</span><span class="sxs-lookup"><span data-stu-id="e4e83-104">List user transitive memberOf</span></span>

> <span data-ttu-id="e4e83-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4e83-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4e83-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4e83-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4e83-107">Abrufen von Gruppen, Directory Rollen und administrative Einheiten, denen der Benutzer Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="e4e83-107">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="e4e83-108">Diese API-Anforderung ist transitiv und alle Gruppen, die, denen der Benutzer ein geschachtelte Mitglied ist, wird ebenfalls zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4e83-108">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4e83-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4e83-109">Permissions</span></span>

<span data-ttu-id="e4e83-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4e83-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e83-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4e83-112">Permission type</span></span>      | <span data-ttu-id="e4e83-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4e83-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4e83-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4e83-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e4e83-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4e83-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4e83-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4e83-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4e83-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4e83-117">Not supported.</span></span>    |
|<span data-ttu-id="e4e83-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4e83-118">Application</span></span> | <span data-ttu-id="e4e83-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e83-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4e83-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4e83-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4e83-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e4e83-121">Optional query parameters</span></span>

<span data-ttu-id="e4e83-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e4e83-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4e83-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4e83-123">Request headers</span></span>

| <span data-ttu-id="e4e83-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4e83-124">Header</span></span>       | <span data-ttu-id="e4e83-125">Wert</span><span class="sxs-lookup"><span data-stu-id="e4e83-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4e83-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e83-126">Authorization</span></span>  | <span data-ttu-id="e4e83-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4e83-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4e83-129">Accept</span><span class="sxs-lookup"><span data-stu-id="e4e83-129">Accept</span></span>  | <span data-ttu-id="e4e83-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e83-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e83-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4e83-131">Request body</span></span>

<span data-ttu-id="e4e83-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e4e83-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4e83-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4e83-133">Response</span></span>

<span data-ttu-id="e4e83-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4e83-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e83-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4e83-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e83-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4e83-136">Request</span></span>

<span data-ttu-id="e4e83-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4e83-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="e4e83-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4e83-138">Response</span></span>

<span data-ttu-id="e4e83-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4e83-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->