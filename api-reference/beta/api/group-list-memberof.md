---
title: Liste Gruppe Mitglied
description: Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein direktes Mitglied ist.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3a9f35774bd626a8ed33ba351c7e388579aebf80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970850"
---
# <a name="list-group-memberof"></a><span data-ttu-id="0bfe9-103">Liste Gruppe Mitglied</span><span class="sxs-lookup"><span data-stu-id="0bfe9-103">List group memberOf</span></span>

> <span data-ttu-id="0bfe9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bfe9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0bfe9-106">Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-106">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="0bfe9-107">Dieser Vorgang ist nicht transitiv.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-107">This operation is not transitive.</span></span> <span data-ttu-id="0bfe9-108">Im Gegensatz zum Abrufen eines Benutzers Office 365-Gruppen, die alle Arten von Gruppen, zurückgegebene nicht nur die Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0bfe9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0bfe9-109">Permissions</span></span>

<span data-ttu-id="0bfe9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bfe9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bfe9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bfe9-112">Permission type</span></span>      | <span data-ttu-id="0bfe9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bfe9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bfe9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bfe9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0bfe9-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bfe9-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bfe9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bfe9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bfe9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bfe9-117">Not supported.</span></span>    |
|<span data-ttu-id="0bfe9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bfe9-118">Application</span></span> | <span data-ttu-id="0bfe9-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bfe9-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bfe9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bfe9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0bfe9-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0bfe9-121">Optional query parameters</span></span>
<span data-ttu-id="0bfe9-122">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bfe9-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bfe9-123">Request headers</span></span>
| <span data-ttu-id="0bfe9-124">Name</span><span class="sxs-lookup"><span data-stu-id="0bfe9-124">Name</span></span>       | <span data-ttu-id="0bfe9-125">Typ</span><span class="sxs-lookup"><span data-stu-id="0bfe9-125">Type</span></span> | <span data-ttu-id="0bfe9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bfe9-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0bfe9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bfe9-127">Authorization</span></span>  | <span data-ttu-id="0bfe9-128">string</span><span class="sxs-lookup"><span data-stu-id="0bfe9-128">string</span></span>  | <span data-ttu-id="0bfe9-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bfe9-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bfe9-131">Request body</span></span>
<span data-ttu-id="0bfe9-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bfe9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bfe9-133">Response</span></span>
<span data-ttu-id="0bfe9-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bfe9-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bfe9-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bfe9-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bfe9-136">Request</span></span>

<span data-ttu-id="0bfe9-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="0bfe9-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bfe9-138">Response</span></span>

<span data-ttu-id="0bfe9-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-139">The following is an example of the response.</span></span>
><span data-ttu-id="0bfe9-140">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0bfe9-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0bfe9-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
