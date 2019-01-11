---
title: Abrufen von governanceRoleDefinition
description: Abrufen der Eigenschaften und Beziehungen zwischen einer GovernanceRoleDefinition.
localization_priority: Normal
ms.openlocfilehash: 99f19e1942c198259d9df7dd6e0f9e5a7685bc09
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865065"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="fd864-103">Abrufen von governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="fd864-103">Get governanceRoleDefinition</span></span>

> <span data-ttu-id="fd864-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd864-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd864-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd864-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd864-106">Abrufen der Eigenschaften und Beziehungen zwischen einer [GovernanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fd864-106">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd864-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd864-107">Permissions</span></span>
<span data-ttu-id="fd864-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd864-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd864-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd864-110">Permission type</span></span>      | <span data-ttu-id="fd864-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd864-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd864-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd864-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd864-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="fd864-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="fd864-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd864-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd864-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd864-115">Not supported.</span></span>    |
|<span data-ttu-id="fd864-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd864-116">Application</span></span> | <span data-ttu-id="fd864-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="fd864-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="fd864-118">Neben den Berechtigungsbereich benötigt diese API den Requestor mindestens eine rollenzuweisung für die Ressource verfügen, die die [GovernanceRoleDefinition](../resources/governanceroledefinition.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="fd864-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd864-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd864-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd864-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd864-120">Optional query parameters</span></span>
<span data-ttu-id="fd864-121">Diese Methode führt **kein** Support den [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="fd864-121">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd864-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd864-122">Request headers</span></span>
| <span data-ttu-id="fd864-123">Name</span><span class="sxs-lookup"><span data-stu-id="fd864-123">Name</span></span>      |<span data-ttu-id="fd864-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd864-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd864-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd864-125">Authorization</span></span>  | <span data-ttu-id="fd864-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fd864-126">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="fd864-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd864-127">Request body</span></span>
<span data-ttu-id="fd864-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd864-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fd864-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd864-129">Response</span></span>
<span data-ttu-id="fd864-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GovernanceRoleDefinition](../resources/governanceroledefinition.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fd864-130">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd864-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd864-131">Example</span></span>
<span data-ttu-id="fd864-132">In diesem Beispiel wird gezeigt, wie Details der Rollendefinition DNS-Zone Mitwirkender im Abonnement Wingtip Toys - "Bemerkungen" abgerufen.</span><span class="sxs-lookup"><span data-stu-id="fd864-132">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="fd864-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd864-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="fd864-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd864-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
