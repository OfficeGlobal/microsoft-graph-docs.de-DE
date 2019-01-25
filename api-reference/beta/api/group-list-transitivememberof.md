---
title: Liste Gruppe transitive Mitglied
description: Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist.  Dieser Vorgang ist transitiv und werden auch alle Gruppen, die diese Gruppen gehört geschachtelte aufgenommen. Im Gegensatz zum Abrufen eines Benutzers Office 365-Gruppen, die alle Arten von Gruppen, zurückgegebene nicht nur die Office 365-Gruppen.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 95d191973a327e6b3e1b0c7e692e0d581744e0ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515832"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="64d4e-105">Liste Gruppe transitive Mitglied</span><span class="sxs-lookup"><span data-stu-id="64d4e-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64d4e-106">Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="64d4e-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="64d4e-107">Dieser Vorgang ist transitiv und werden auch alle Gruppen, die diese Gruppen gehört geschachtelte aufgenommen.</span><span class="sxs-lookup"><span data-stu-id="64d4e-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="64d4e-108">Im Gegensatz zum Abrufen eines Benutzers Office 365-Gruppen, die alle Arten von Gruppen, zurückgegebene nicht nur die Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="64d4e-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="64d4e-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64d4e-109">Permissions</span></span>

<span data-ttu-id="64d4e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64d4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64d4e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64d4e-112">Permission type</span></span>      | <span data-ttu-id="64d4e-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64d4e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64d4e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64d4e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="64d4e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64d4e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64d4e-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64d4e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64d4e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64d4e-117">Not supported.</span></span>    |
|<span data-ttu-id="64d4e-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64d4e-118">Application</span></span> | <span data-ttu-id="64d4e-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d4e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64d4e-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64d4e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64d4e-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="64d4e-121">Optional query parameters</span></span>
<span data-ttu-id="64d4e-122">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64d4e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64d4e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64d4e-123">Request headers</span></span>
| <span data-ttu-id="64d4e-124">Name</span><span class="sxs-lookup"><span data-stu-id="64d4e-124">Name</span></span>       | <span data-ttu-id="64d4e-125">Typ</span><span class="sxs-lookup"><span data-stu-id="64d4e-125">Type</span></span> | <span data-ttu-id="64d4e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64d4e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="64d4e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="64d4e-127">Authorization</span></span>  | <span data-ttu-id="64d4e-128">string</span><span class="sxs-lookup"><span data-stu-id="64d4e-128">string</span></span>  | <span data-ttu-id="64d4e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64d4e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64d4e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64d4e-131">Request body</span></span>
<span data-ttu-id="64d4e-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64d4e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64d4e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="64d4e-133">Response</span></span>
<span data-ttu-id="64d4e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64d4e-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64d4e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64d4e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="64d4e-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64d4e-136">Request</span></span>
<span data-ttu-id="64d4e-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64d4e-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="64d4e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="64d4e-138">Response</span></span>

<span data-ttu-id="64d4e-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64d4e-139">The following is an example of the response.</span></span>
><span data-ttu-id="64d4e-140">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="64d4e-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="64d4e-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="64d4e-141">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
