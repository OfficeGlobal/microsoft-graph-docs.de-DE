---
title: Abrufen von governanceResource
description: Rufen Sie die Eigenschaften und die Beziehungen eines GovernanceResource-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: be24fb8822101f7a67a5bd60f1fe018cf1a08f6b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522147"
---
# <a name="get-governanceresource"></a><span data-ttu-id="eb302-103">Abrufen von governanceResource</span><span class="sxs-lookup"><span data-stu-id="eb302-103">Get governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb302-104">Rufen Sie die Eigenschaften und die Beziehungen eines [GovernanceResource](../resources/governanceresource.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="eb302-104">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb302-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb302-105">Permissions</span></span>
<span data-ttu-id="eb302-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb302-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb302-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb302-108">Permission type</span></span>      | <span data-ttu-id="eb302-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb302-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb302-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb302-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb302-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="eb302-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="eb302-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb302-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb302-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb302-113">Not supported.</span></span>    |
|<span data-ttu-id="eb302-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb302-114">Application</span></span> | <span data-ttu-id="eb302-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="eb302-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="eb302-116">Neben den Berechtigungsbereich benötigt diese API den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="eb302-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="eb302-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb302-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb302-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="eb302-118">Optional query parameters</span></span>
<span data-ttu-id="eb302-119">Diese Methode unterstützt **nur** das `$select` und `$expand` [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="eb302-119">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb302-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb302-120">Request headers</span></span>
| <span data-ttu-id="eb302-121">Name</span><span class="sxs-lookup"><span data-stu-id="eb302-121">Name</span></span>      |<span data-ttu-id="eb302-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb302-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb302-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb302-123">Authorization</span></span>  | <span data-ttu-id="eb302-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eb302-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb302-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb302-125">Request body</span></span>
<span data-ttu-id="eb302-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb302-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eb302-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb302-127">Response</span></span>
<span data-ttu-id="eb302-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GovernanceResource](../resources/governanceresource.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="eb302-128">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb302-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb302-129">Example</span></span>
<span data-ttu-id="eb302-130">In diesem Beispiel wird gezeigt, wie die Details des Abonnements Wingtip Toys - "Bemerkungen" (e5e7d29d-5465-45ac-885f-4716a5ee74b5) abgerufen.</span><span class="sxs-lookup"><span data-stu-id="eb302-130">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="eb302-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb302-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="eb302-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb302-132">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
