---
title: Abrufen von governanceResource
description: Rufen Sie die Eigenschaften und die Beziehungen eines GovernanceResource-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 16442ea971a635aedfd89f09c48ffddf14c83b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888032"
---
# <a name="get-governanceresource"></a><span data-ttu-id="3b4b9-103">Abrufen von governanceResource</span><span class="sxs-lookup"><span data-stu-id="3b4b9-103">Get governanceResource</span></span>

> <span data-ttu-id="3b4b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b4b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b4b9-106">Rufen Sie die Eigenschaften und die Beziehungen eines [GovernanceResource](../resources/governanceresource.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b4b9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b4b9-107">Permissions</span></span>
<span data-ttu-id="3b4b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b4b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b4b9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b4b9-110">Permission type</span></span>      | <span data-ttu-id="3b4b9-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b4b9-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b4b9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b4b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b4b9-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3b4b9-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3b4b9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b4b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b4b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b4b9-115">Not supported.</span></span>    |
|<span data-ttu-id="3b4b9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b4b9-116">Application</span></span> | <span data-ttu-id="3b4b9-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3b4b9-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="3b4b9-118">Neben den Berechtigungsbereich benötigt diese API den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="3b4b9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b4b9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b4b9-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3b4b9-120">Optional query parameters</span></span>
<span data-ttu-id="3b4b9-121">Diese Methode unterstützt **nur** das `$select` und `$expand` [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b4b9-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b4b9-122">Request headers</span></span>
| <span data-ttu-id="3b4b9-123">Name</span><span class="sxs-lookup"><span data-stu-id="3b4b9-123">Name</span></span>      |<span data-ttu-id="3b4b9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b4b9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b4b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b4b9-125">Authorization</span></span>  | <span data-ttu-id="3b4b9-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3b4b9-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b4b9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b4b9-127">Request body</span></span>
<span data-ttu-id="3b4b9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3b4b9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b4b9-129">Response</span></span>
<span data-ttu-id="3b4b9-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GovernanceResource](../resources/governanceresource.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b4b9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b4b9-131">Example</span></span>
<span data-ttu-id="3b4b9-132">In diesem Beispiel wird gezeigt, wie die Details des Abonnements Wingtip Toys - "Bemerkungen" (e5e7d29d-5465-45ac-885f-4716a5ee74b5) abgerufen.</span><span class="sxs-lookup"><span data-stu-id="3b4b9-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="3b4b9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b4b9-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="3b4b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b4b9-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
