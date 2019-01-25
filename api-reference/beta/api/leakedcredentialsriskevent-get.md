---
title: Abrufen von leakedCredentialsRiskEvent
description: Rufen Sie die Eigenschaften und die Beziehungen eines Leakedcredentialsriskevent-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: eb7b7ca5ecac02a91c2e9733511cd0a384782bd3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509833"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="86c9d-103">Abrufen von leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="86c9d-103">Get leakedCredentialsRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c9d-104">Rufen Sie die Eigenschaften und die Beziehungen eines Leakedcredentialsriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="86c9d-104">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86c9d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86c9d-105">Permissions</span></span>
<span data-ttu-id="86c9d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c9d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86c9d-108">Permission type</span></span>      | <span data-ttu-id="86c9d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86c9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86c9d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86c9d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86c9d-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c9d-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="86c9d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86c9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c9d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86c9d-113">Not supported.</span></span>    |
|<span data-ttu-id="86c9d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86c9d-114">Application</span></span> | <span data-ttu-id="86c9d-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c9d-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86c9d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86c9d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="86c9d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86c9d-117">Request headers</span></span>
| <span data-ttu-id="86c9d-118">Name</span><span class="sxs-lookup"><span data-stu-id="86c9d-118">Name</span></span>      |<span data-ttu-id="86c9d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86c9d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86c9d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="86c9d-120">Authorization</span></span>  | <span data-ttu-id="86c9d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86c9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86c9d-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="86c9d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="86c9d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="86c9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c9d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86c9d-126">Request body</span></span>
<span data-ttu-id="86c9d-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="86c9d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86c9d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="86c9d-128">Response</span></span>

<span data-ttu-id="86c9d-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [LeakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="86c9d-129">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86c9d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86c9d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86c9d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86c9d-131">Request</span></span>
<span data-ttu-id="86c9d-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86c9d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="86c9d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="86c9d-133">Response</span></span>
<span data-ttu-id="86c9d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86c9d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "closedDateTime": null,
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "active",
  "riskLevel": "high",
  "riskType": "LeakedCredentialsRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/leakedcredentialsriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
