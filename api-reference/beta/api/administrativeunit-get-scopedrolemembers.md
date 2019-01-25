---
title: Abrufen einer scopedRoleMember
description: Rufen Sie eine bestimmte ScopedRoleMembership Ressource ab.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e961097184730922aebd4348f88b8570d5c24ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525990"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="e04dc-103">Abrufen einer scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="e04dc-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e04dc-104">Rufen Sie eine bestimmte [ScopedRoleMembership](../resources/scopedrolemembership.md) Ressource ab.</span><span class="sxs-lookup"><span data-stu-id="e04dc-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="e04dc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e04dc-105">Permissions</span></span>
<span data-ttu-id="e04dc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e04dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e04dc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e04dc-108">Permission type</span></span>      | <span data-ttu-id="e04dc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e04dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e04dc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e04dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e04dc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e04dc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e04dc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e04dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e04dc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e04dc-113">Not supported.</span></span>    |
|<span data-ttu-id="e04dc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e04dc-114">Application</span></span> | <span data-ttu-id="e04dc-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04dc-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e04dc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e04dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e04dc-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e04dc-117">Optional query parameters</span></span>
<span data-ttu-id="e04dc-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e04dc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e04dc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e04dc-119">Request headers</span></span>
| <span data-ttu-id="e04dc-120">Name</span><span class="sxs-lookup"><span data-stu-id="e04dc-120">Name</span></span>      |<span data-ttu-id="e04dc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e04dc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e04dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e04dc-122">Authorization</span></span>  | <span data-ttu-id="e04dc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e04dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e04dc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e04dc-125">Request body</span></span>
<span data-ttu-id="e04dc-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e04dc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e04dc-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e04dc-127">Response</span></span>

<span data-ttu-id="e04dc-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und das angeforderte [ScopedRoleMembership](../resources/scopedrolemembership.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e04dc-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e04dc-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e04dc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e04dc-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e04dc-130">Request</span></span>
<span data-ttu-id="e04dc-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e04dc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="e04dc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e04dc-132">Response</span></span>
<span data-ttu-id="e04dc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e04dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
