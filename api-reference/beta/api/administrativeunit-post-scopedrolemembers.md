---
title: Hinzufügen einer scopedRoleMember
description: 'Fügen Sie eine neue ScopedRoleMembership hinzu. Hinweis: Nur die *Benutzer Kontoadministrator* und *Helpdeskadministrator* Rollen werden derzeit für bezogenen Rollenmitgliedschaften unterstützt.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f94c66bd804d2771987ee58539abdbe073abc03
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640357"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="9590b-104">Hinzufügen einer scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="9590b-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9590b-105">Fügen Sie eine neue [ScopedRoleMembership](../resources/scopedrolemembership.md)hinzu.</span><span class="sxs-lookup"><span data-stu-id="9590b-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="9590b-106">Hinweis: Nur die *Benutzer Kontoadministrator* und *Helpdeskadministrator* Rollen werden derzeit für bezogenen Rollenmitgliedschaften unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9590b-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="9590b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9590b-107">Permissions</span></span>
<span data-ttu-id="9590b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9590b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9590b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9590b-110">Permission type</span></span>      | <span data-ttu-id="9590b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9590b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9590b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9590b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9590b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9590b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9590b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9590b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9590b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9590b-115">Not supported.</span></span>    |
|<span data-ttu-id="9590b-116">Application</span><span class="sxs-lookup"><span data-stu-id="9590b-116">Application</span></span> | <span data-ttu-id="9590b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9590b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9590b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9590b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="9590b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9590b-119">Request headers</span></span>
| <span data-ttu-id="9590b-120">Name</span><span class="sxs-lookup"><span data-stu-id="9590b-120">Name</span></span>      |<span data-ttu-id="9590b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9590b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9590b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9590b-122">Authorization</span></span>  | <span data-ttu-id="9590b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9590b-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9590b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9590b-125">Request body</span></span>
<span data-ttu-id="9590b-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ScopedRoleMembership](../resources/scopedrolemembership.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9590b-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9590b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9590b-127">Response</span></span>

<span data-ttu-id="9590b-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [ScopedRoleMembership](../resources/scopedrolemembership.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9590b-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9590b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9590b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9590b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9590b-130">Request</span></span>
<span data-ttu-id="9590b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9590b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
<span data-ttu-id="9590b-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ScopedRoleMembership](../resources/scopedrolemembership.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9590b-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9590b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9590b-133">Response</span></span>
<span data-ttu-id="9590b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9590b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships/$entity",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value",
    "displayName": "displayName-value",
    "userPrincipalName": "userPrincipalName-value"
  },
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
