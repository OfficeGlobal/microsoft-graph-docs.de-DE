---
title: Liste unfamiliarLocationRiskEvents
description: Abrufen einer Liste von Unfamiliarlocationriskevent-Objekten.
localization_priority: Normal
ms.openlocfilehash: 10a56b27cd29bb674dbbd97c522ac0b92671b7eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526963"
---
# <a name="list-unfamiliarlocationriskevents"></a><span data-ttu-id="89d21-103">Liste unfamiliarLocationRiskEvents</span><span class="sxs-lookup"><span data-stu-id="89d21-103">List unfamiliarLocationRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89d21-104">Abrufen einer Liste von Unfamiliarlocationriskevent-Objekten.</span><span class="sxs-lookup"><span data-stu-id="89d21-104">Retrieve a list of unfamiliarlocationriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="89d21-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="89d21-105">Permissions</span></span>
<span data-ttu-id="89d21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89d21-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89d21-108">Permission type</span></span>      | <span data-ttu-id="89d21-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89d21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89d21-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89d21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89d21-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d21-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="89d21-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89d21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89d21-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89d21-113">Not supported.</span></span>    |
|<span data-ttu-id="89d21-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89d21-114">Application</span></span> | <span data-ttu-id="89d21-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d21-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89d21-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89d21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="89d21-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89d21-117">Request headers</span></span>
| <span data-ttu-id="89d21-118">Name</span><span class="sxs-lookup"><span data-stu-id="89d21-118">Name</span></span>      |<span data-ttu-id="89d21-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89d21-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89d21-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="89d21-120">Authorization</span></span>  | <span data-ttu-id="89d21-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89d21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89d21-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="89d21-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="89d21-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="89d21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d21-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89d21-126">Request body</span></span>
<span data-ttu-id="89d21-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="89d21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89d21-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="89d21-128">Response</span></span>

<span data-ttu-id="89d21-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [UnfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) .</span><span class="sxs-lookup"><span data-stu-id="89d21-129">If successful, this method returns a `200 OK` response code and collection of [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89d21-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89d21-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89d21-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89d21-131">Request</span></span>
<span data-ttu-id="89d21-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89d21-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents
```
##### <a name="response"></a><span data-ttu-id="89d21-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="89d21-133">Response</span></span>
<span data-ttu-id="89d21-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89d21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List unfamiliarLocationRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/unfamiliarlocationriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
