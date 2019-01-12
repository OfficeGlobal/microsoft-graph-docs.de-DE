---
title: Hinzufügen einer scopedRoleMember
description: 'Fügen Sie eine neue ScopedRoleMembership hinzu. Hinweis: Nur die *Benutzer Kontoadministrator* und *Helpdeskadministrator* Rollen werden derzeit für bezogenen Rollenmitgliedschaften unterstützt.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6dce85d891c9d124d1d57d14a8a7309fb766b895
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936683"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="6a509-104">Hinzufügen einer scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="6a509-104">Add a scopedRoleMember</span></span>

> <span data-ttu-id="6a509-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a509-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a509-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a509-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a509-107">Fügen Sie eine neue [ScopedRoleMembership](../resources/scopedrolemembership.md)hinzu.</span><span class="sxs-lookup"><span data-stu-id="6a509-107">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="6a509-108">Hinweis: Nur die *Benutzer Kontoadministrator* und *Helpdeskadministrator* Rollen werden derzeit für bezogenen Rollenmitgliedschaften unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a509-108">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a509-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a509-109">Permissions</span></span>
<span data-ttu-id="6a509-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a509-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6a509-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a509-112">Permission type</span></span>      | <span data-ttu-id="6a509-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a509-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a509-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a509-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6a509-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a509-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a509-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a509-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a509-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a509-117">Not supported.</span></span>    |
|<span data-ttu-id="6a509-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a509-118">Application</span></span> | <span data-ttu-id="6a509-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a509-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a509-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a509-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="6a509-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a509-121">Request headers</span></span>
| <span data-ttu-id="6a509-122">Name</span><span class="sxs-lookup"><span data-stu-id="6a509-122">Name</span></span>      |<span data-ttu-id="6a509-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a509-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a509-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a509-124">Authorization</span></span>  | <span data-ttu-id="6a509-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a509-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a509-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a509-127">Request body</span></span>
<span data-ttu-id="6a509-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ScopedRoleMembership](../resources/scopedrolemembership.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a509-128">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6a509-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a509-129">Response</span></span>

<span data-ttu-id="6a509-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [ScopedRoleMembership](../resources/scopedrolemembership.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6a509-130">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a509-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a509-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a509-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a509-132">Request</span></span>
<span data-ttu-id="6a509-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a509-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="6a509-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ScopedRoleMembership](../resources/scopedrolemembership.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a509-134">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6a509-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a509-135">Response</span></span>
<span data-ttu-id="6a509-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a509-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
