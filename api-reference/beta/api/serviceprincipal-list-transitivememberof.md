---
title: Liste ServicePrincipal transitive Mitglied
description: Rufen Sie die Gruppen und Directory Rollen, denen dieser Dienst principal ein Mitglied ist. Dieser Vorgang ist transitiv und schließt alle Gruppen, denen dieser Dienst principal geschachtelte Mitglied ist.
localization_priority: Normal
ms.openlocfilehash: 4588f5ea4c6190b3743988c1d97bfd5caacbfaa4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526228"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="cfff0-104">Liste ServicePrincipal transitive Mitglied</span><span class="sxs-lookup"><span data-stu-id="cfff0-104">List servicePrincipal transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfff0-105">Rufen Sie die Gruppen und Directory Rollen, denen dieser Dienst principal ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="cfff0-105">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="cfff0-106">Dieser Vorgang ist transitiv und schließt alle Gruppen, denen dieser Dienst principal geschachtelte Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="cfff0-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfff0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cfff0-107">Permissions</span></span>
<span data-ttu-id="cfff0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfff0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfff0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cfff0-110">Permission type</span></span>      | <span data-ttu-id="cfff0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cfff0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfff0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cfff0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cfff0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfff0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cfff0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cfff0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfff0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfff0-115">Not supported.</span></span>    |
|<span data-ttu-id="cfff0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cfff0-116">Application</span></span> | <span data-ttu-id="cfff0-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfff0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfff0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfff0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cfff0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cfff0-119">Optional query parameters</span></span>
<span data-ttu-id="cfff0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cfff0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfff0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cfff0-121">Request headers</span></span>
| <span data-ttu-id="cfff0-122">Name</span><span class="sxs-lookup"><span data-stu-id="cfff0-122">Name</span></span>       | <span data-ttu-id="cfff0-123">Typ</span><span class="sxs-lookup"><span data-stu-id="cfff0-123">Type</span></span> | <span data-ttu-id="cfff0-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfff0-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cfff0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfff0-125">Authorization</span></span>  | <span data-ttu-id="cfff0-126">string</span><span class="sxs-lookup"><span data-stu-id="cfff0-126">string</span></span>  | <span data-ttu-id="cfff0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfff0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfff0-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cfff0-129">Request body</span></span>
<span data-ttu-id="cfff0-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cfff0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfff0-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfff0-131">Response</span></span>

<span data-ttu-id="cfff0-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfff0-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfff0-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cfff0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfff0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfff0-134">Request</span></span>

<span data-ttu-id="cfff0-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cfff0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="cfff0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfff0-136">Response</span></span>

<span data-ttu-id="cfff0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfff0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
