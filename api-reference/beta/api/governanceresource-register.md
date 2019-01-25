---
title: GovernanceResource registrieren
description: Registrieren Sie ein Objekt nicht verwalteten GovernanceResource in PIM.
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519045"
---
# <a name="register-governanceresource"></a><span data-ttu-id="0ce34-103">GovernanceResource registrieren</span><span class="sxs-lookup"><span data-stu-id="0ce34-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ce34-104">Registrieren Sie ein Objekt nicht verwalteten [GovernanceResource](../resources/governanceresource.md) in privilegierten Identity Management.</span><span class="sxs-lookup"><span data-stu-id="0ce34-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ce34-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0ce34-105">Permissions</span></span>
<span data-ttu-id="0ce34-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ce34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="0ce34-108">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine aktive Rolle-Zuordnung für die Ressource verfügen.</span><span class="sxs-lookup"><span data-stu-id="0ce34-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="0ce34-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ce34-109">Permission type</span></span>      | <span data-ttu-id="0ce34-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0ce34-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce34-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ce34-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ce34-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0ce34-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0ce34-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ce34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce34-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ce34-114">Not supported.</span></span>    |
|<span data-ttu-id="0ce34-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ce34-115">Application</span></span> | <span data-ttu-id="0ce34-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0ce34-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ce34-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ce34-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="0ce34-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0ce34-118">Optional query parameters</span></span>
<span data-ttu-id="0ce34-119">Diese Methode unterstützt die **nur** die `$select` und `$expand` [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="0ce34-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="0ce34-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ce34-120">Request headers</span></span>
| <span data-ttu-id="0ce34-121">Name</span><span class="sxs-lookup"><span data-stu-id="0ce34-121">Name</span></span>      |<span data-ttu-id="0ce34-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ce34-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ce34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce34-123">Authorization</span></span>  | <span data-ttu-id="0ce34-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ce34-124">Bearer {code}</span></span>|
| <span data-ttu-id="0ce34-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="0ce34-125">Content-type</span></span>  | <span data-ttu-id="0ce34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ce34-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="0ce34-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ce34-127">Request body</span></span>

|<span data-ttu-id="0ce34-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="0ce34-128">Parameters</span></span>      |<span data-ttu-id="0ce34-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0ce34-129">Type</span></span>                 |<span data-ttu-id="0ce34-130">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ce34-130">Required</span></span> |<span data-ttu-id="0ce34-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ce34-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="0ce34-132">externalId</span><span class="sxs-lookup"><span data-stu-id="0ce34-132">externalId</span></span>    |<span data-ttu-id="0ce34-133">String</span><span class="sxs-lookup"><span data-stu-id="0ce34-133">String</span></span>                 |<span data-ttu-id="0ce34-134">✓</span><span class="sxs-lookup"><span data-stu-id="0ce34-134">✓</span></span>        |<span data-ttu-id="0ce34-135">Die ExternalId der Ressource in PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="0ce34-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="0ce34-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ce34-136">Response</span></span>
<span data-ttu-id="0ce34-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwort.</span><span class="sxs-lookup"><span data-stu-id="0ce34-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="0ce34-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ce34-138">Example</span></span>
<span data-ttu-id="0ce34-139">In diesem Beispiel wird gezeigt, wie ein Azure-Abonnement Wingtip Toys - "Bemerkungen" registriert.</span><span class="sxs-lookup"><span data-stu-id="0ce34-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="0ce34-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ce34-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="0ce34-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ce34-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
