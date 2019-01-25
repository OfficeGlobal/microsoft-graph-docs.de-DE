---
title: Abrufen von locatedRiskEvent
description: Rufen Sie die Eigenschaften und die Beziehungen eines Locatedriskevent-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: aee63e3f9cbb90f839d3eaebf5ec37b2f5b53042
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509231"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="60abc-103">Abrufen von locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="60abc-103">Get locatedRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60abc-104">Rufen Sie die Eigenschaften und die Beziehungen eines Locatedriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="60abc-104">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60abc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60abc-105">Permissions</span></span>
<span data-ttu-id="60abc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60abc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60abc-108">Permission type</span></span>      | <span data-ttu-id="60abc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60abc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60abc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60abc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60abc-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="60abc-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="60abc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60abc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60abc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60abc-113">Not supported.</span></span>    |
|<span data-ttu-id="60abc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60abc-114">Application</span></span> | <span data-ttu-id="60abc-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="60abc-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60abc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60abc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60abc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60abc-117">Request headers</span></span>
| <span data-ttu-id="60abc-118">Name</span><span class="sxs-lookup"><span data-stu-id="60abc-118">Name</span></span>      |<span data-ttu-id="60abc-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60abc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60abc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60abc-120">Authorization</span></span>  | <span data-ttu-id="60abc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60abc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60abc-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="60abc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="60abc-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="60abc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60abc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60abc-126">Request body</span></span>
<span data-ttu-id="60abc-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="60abc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60abc-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="60abc-128">Response</span></span>

<span data-ttu-id="60abc-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [LocatedRiskEvent](../resources/locatedriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="60abc-129">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60abc-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60abc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60abc-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60abc-131">Request</span></span>
<span data-ttu-id="60abc-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60abc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="60abc-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="60abc-133">Response</span></span>
<span data-ttu-id="60abc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60abc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.locatedRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "a6653179-3c7b-4e99-bb4c-dddeb18adfc1",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/locatedriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
