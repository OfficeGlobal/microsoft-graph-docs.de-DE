---
title: Abrufen von suspiciousIpRiskEvent
description: Rufen Sie die Eigenschaften und die Beziehungen eines Suspiciousipriskevent-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 64218e000eb32065a65d68d69e3735caa11b3ca0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521558"
---
# <a name="get-suspiciousipriskevent"></a><span data-ttu-id="4962f-103">Abrufen von suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4962f-103">Get suspiciousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4962f-104">Rufen Sie die Eigenschaften und die Beziehungen eines Suspiciousipriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="4962f-104">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4962f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4962f-105">Permissions</span></span>
<span data-ttu-id="4962f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4962f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4962f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4962f-108">Permission type</span></span>      | <span data-ttu-id="4962f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4962f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4962f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4962f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4962f-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="4962f-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="4962f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4962f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4962f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4962f-113">Not supported.</span></span>    |
|<span data-ttu-id="4962f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4962f-114">Application</span></span> | <span data-ttu-id="4962f-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="4962f-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4962f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4962f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4962f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4962f-117">Request headers</span></span>
| <span data-ttu-id="4962f-118">Name</span><span class="sxs-lookup"><span data-stu-id="4962f-118">Name</span></span>      |<span data-ttu-id="4962f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4962f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4962f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4962f-120">Authorization</span></span>  | <span data-ttu-id="4962f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4962f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4962f-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4962f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4962f-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4962f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4962f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4962f-126">Request body</span></span>
<span data-ttu-id="4962f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4962f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4962f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4962f-128">Response</span></span>

<span data-ttu-id="4962f-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [SuspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4962f-129">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4962f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4962f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4962f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4962f-131">Request</span></span>
<span data-ttu-id="4962f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4962f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="4962f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4962f-133">Response</span></span>
<span data-ttu-id="4962f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4962f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": null,
  "createdDateTime": "2016-02-03T06:08:35.123512Z",
  "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
  "ipAddress": "95.31.18.119",
  "location": "Moskva, Russia, RU",
  "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
  "riskEventStatus": "active",
  "riskLevel": "low",
  "riskType": "SuspiciousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/suspiciousipriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
