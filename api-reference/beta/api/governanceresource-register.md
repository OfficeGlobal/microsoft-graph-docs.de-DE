---
title: GovernanceResource registrieren
description: Registrieren Sie ein Objekt nicht verwalteten GovernanceResource in PIM.
ms.openlocfilehash: 53452202b58c2d2187b6876eabfaae1ae646710d
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27195297"
---
# <a name="register-governanceresource"></a><span data-ttu-id="6e0cb-103">GovernanceResource registrieren</span><span class="sxs-lookup"><span data-stu-id="6e0cb-103">Register governanceResource</span></span>

> <span data-ttu-id="6e0cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e0cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e0cb-106">Registrieren Sie ein Objekt nicht verwalteten [GovernanceResource](../resources/governanceresource.md) in privilegierten Identity Management.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-106">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e0cb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e0cb-107">Permissions</span></span>
<span data-ttu-id="6e0cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e0cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="6e0cb-110">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine aktive Rolle-Zuordnung für die Ressource verfügen.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-110">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="6e0cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e0cb-111">Permission type</span></span>      | <span data-ttu-id="6e0cb-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e0cb-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e0cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e0cb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6e0cb-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6e0cb-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6e0cb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e0cb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e0cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e0cb-116">Not supported.</span></span>    |
|<span data-ttu-id="6e0cb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e0cb-117">Application</span></span> | <span data-ttu-id="6e0cb-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6e0cb-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e0cb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e0cb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="6e0cb-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6e0cb-120">Optional query parameters</span></span>
<span data-ttu-id="6e0cb-121">Diese Methode unterstützt die **nur** die `$select` und `$expand` [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-121">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="6e0cb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e0cb-122">Request headers</span></span>
| <span data-ttu-id="6e0cb-123">Name</span><span class="sxs-lookup"><span data-stu-id="6e0cb-123">Name</span></span>      |<span data-ttu-id="6e0cb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e0cb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e0cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e0cb-125">Authorization</span></span>  | <span data-ttu-id="6e0cb-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6e0cb-126">Bearer {code}</span></span>|
| <span data-ttu-id="6e0cb-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="6e0cb-127">Content-type</span></span>  | <span data-ttu-id="6e0cb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6e0cb-128">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="6e0cb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e0cb-129">Request body</span></span>

|<span data-ttu-id="6e0cb-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="6e0cb-130">Parameters</span></span>      |<span data-ttu-id="6e0cb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6e0cb-131">Type</span></span>                 |<span data-ttu-id="6e0cb-132">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="6e0cb-132">Required</span></span> |<span data-ttu-id="6e0cb-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e0cb-133">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="6e0cb-134">externalId</span><span class="sxs-lookup"><span data-stu-id="6e0cb-134">externalId</span></span>    |<span data-ttu-id="6e0cb-135">String</span><span class="sxs-lookup"><span data-stu-id="6e0cb-135">String</span></span>                 |<span data-ttu-id="6e0cb-136">✓</span><span class="sxs-lookup"><span data-stu-id="6e0cb-136">✓</span></span>        |<span data-ttu-id="6e0cb-137">Die ExternalId der Ressource in PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-137">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="6e0cb-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e0cb-138">Response</span></span>
<span data-ttu-id="6e0cb-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-139">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="6e0cb-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e0cb-140">Example</span></span>
<span data-ttu-id="6e0cb-141">In diesem Beispiel wird gezeigt, wie ein Azure-Abonnement Wingtip Toys - "Bemerkungen" registriert.</span><span class="sxs-lookup"><span data-stu-id="6e0cb-141">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="6e0cb-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e0cb-142">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="6e0cb-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e0cb-143">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
