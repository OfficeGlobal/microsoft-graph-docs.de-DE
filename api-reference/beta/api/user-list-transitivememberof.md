---
title: Liste Benutzer transitive Mitglied
description: Abrufen von Gruppen, Directory Rollen und administrative Einheiten, denen der Benutzer Mitglied ist. Diese API-Anforderung ist transitiv und alle Gruppen, die, denen der Benutzer ein geschachtelte Mitglied ist, wird ebenfalls zurückgegeben.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4977d06b05b7b8d860023640f1e413afa3c3c64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953709"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="c8e9e-104">Liste Benutzer transitive Mitglied</span><span class="sxs-lookup"><span data-stu-id="c8e9e-104">List user transitive memberOf</span></span>

> <span data-ttu-id="c8e9e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8e9e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8e9e-107">Abrufen von Gruppen, Directory Rollen und administrative Einheiten, denen der Benutzer Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-107">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="c8e9e-108">Diese API-Anforderung ist transitiv und alle Gruppen, die, denen der Benutzer ein geschachtelte Mitglied ist, wird ebenfalls zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-108">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e9e-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8e9e-109">Permissions</span></span>

<span data-ttu-id="c8e9e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e9e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e9e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8e9e-112">Permission type</span></span>      | <span data-ttu-id="c8e9e-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8e9e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8e9e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8e9e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c8e9e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8e9e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8e9e-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8e9e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e9e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8e9e-117">Not supported.</span></span>    |
|<span data-ttu-id="c8e9e-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8e9e-118">Application</span></span> | <span data-ttu-id="c8e9e-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e9e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8e9e-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8e9e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8e9e-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c8e9e-121">Optional query parameters</span></span>

<span data-ttu-id="c8e9e-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8e9e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8e9e-123">Request headers</span></span>

| <span data-ttu-id="c8e9e-124">Header</span><span class="sxs-lookup"><span data-stu-id="c8e9e-124">Header</span></span>       | <span data-ttu-id="c8e9e-125">Wert</span><span class="sxs-lookup"><span data-stu-id="c8e9e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8e9e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8e9e-126">Authorization</span></span>  | <span data-ttu-id="c8e9e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c8e9e-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8e9e-129">Accept</span></span>  | <span data-ttu-id="c8e9e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c8e9e-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e9e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8e9e-131">Request body</span></span>

<span data-ttu-id="c8e9e-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8e9e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8e9e-133">Response</span></span>

<span data-ttu-id="c8e9e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e9e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8e9e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8e9e-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8e9e-136">Request</span></span>

<span data-ttu-id="c8e9e-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="c8e9e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8e9e-138">Response</span></span>

<span data-ttu-id="c8e9e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8e9e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
