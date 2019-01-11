---
title: Liste Gruppe transitive Mitglied
description: Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist.  Dieser Vorgang ist transitiv und werden auch alle Gruppen, die diese Gruppen gehört geschachtelte aufgenommen. Im Gegensatz zum Abrufen eines Benutzers Office 365-Gruppen, die alle Arten von Gruppen, zurückgegebene nicht nur die Office 365-Gruppen.
localization_priority: Normal
ms.openlocfilehash: 2dececa36b96cfae866afe2f03d4ebb926467ae0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887402"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="73b91-105">Liste Gruppe transitive Mitglied</span><span class="sxs-lookup"><span data-stu-id="73b91-105">List group transitive memberOf</span></span>

> <span data-ttu-id="73b91-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="73b91-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73b91-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73b91-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73b91-108">Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="73b91-108">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="73b91-109">Dieser Vorgang ist transitiv und werden auch alle Gruppen, die diese Gruppen gehört geschachtelte aufgenommen.</span><span class="sxs-lookup"><span data-stu-id="73b91-109">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="73b91-110">Im Gegensatz zum Abrufen eines Benutzers Office 365-Gruppen, die alle Arten von Gruppen, zurückgegebene nicht nur die Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="73b91-110">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="73b91-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="73b91-111">Permissions</span></span>

<span data-ttu-id="73b91-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73b91-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73b91-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73b91-114">Permission type</span></span>      | <span data-ttu-id="73b91-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73b91-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b91-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73b91-116">Delegated (work or school account)</span></span> | <span data-ttu-id="73b91-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73b91-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73b91-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73b91-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b91-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73b91-119">Not supported.</span></span>    |
|<span data-ttu-id="73b91-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73b91-120">Application</span></span> | <span data-ttu-id="73b91-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b91-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b91-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73b91-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73b91-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="73b91-123">Optional query parameters</span></span>
<span data-ttu-id="73b91-124">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="73b91-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73b91-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73b91-125">Request headers</span></span>
| <span data-ttu-id="73b91-126">Name</span><span class="sxs-lookup"><span data-stu-id="73b91-126">Name</span></span>       | <span data-ttu-id="73b91-127">Typ</span><span class="sxs-lookup"><span data-stu-id="73b91-127">Type</span></span> | <span data-ttu-id="73b91-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73b91-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73b91-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="73b91-129">Authorization</span></span>  | <span data-ttu-id="73b91-130">string</span><span class="sxs-lookup"><span data-stu-id="73b91-130">string</span></span>  | <span data-ttu-id="73b91-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73b91-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73b91-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73b91-133">Request body</span></span>
<span data-ttu-id="73b91-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="73b91-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b91-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="73b91-135">Response</span></span>
<span data-ttu-id="73b91-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73b91-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b91-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73b91-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="73b91-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73b91-138">Request</span></span>
<span data-ttu-id="73b91-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73b91-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="73b91-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="73b91-140">Response</span></span>

<span data-ttu-id="73b91-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="73b91-141">The following is an example of the response.</span></span>
><span data-ttu-id="73b91-142">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="73b91-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="73b91-143">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="73b91-143">All the properties will be returned from an actual call.</span></span>
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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
