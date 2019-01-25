---
title: Abrufen von anonymousIpRiskEvent
description: Rufen Sie die Eigenschaften und die Beziehungen eines Anonymousipriskevent-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: c306593d55792035377d18ad1888f5a4ca707aa6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519115"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="665ba-103">Abrufen von anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="665ba-103">Get anonymousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="665ba-104">Rufen Sie die Eigenschaften und die Beziehungen eines Anonymousipriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="665ba-104">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="665ba-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="665ba-105">Permissions</span></span>
<span data-ttu-id="665ba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="665ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="665ba-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="665ba-108">Permission type</span></span>      | <span data-ttu-id="665ba-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="665ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="665ba-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="665ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="665ba-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="665ba-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="665ba-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="665ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="665ba-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="665ba-113">Not supported.</span></span>    |
|<span data-ttu-id="665ba-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="665ba-114">Application</span></span> | <span data-ttu-id="665ba-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="665ba-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="665ba-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="665ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="665ba-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="665ba-117">Request headers</span></span>
| <span data-ttu-id="665ba-118">Name</span><span class="sxs-lookup"><span data-stu-id="665ba-118">Name</span></span>      |<span data-ttu-id="665ba-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="665ba-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="665ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="665ba-120">Authorization</span></span>  | <span data-ttu-id="665ba-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="665ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="665ba-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="665ba-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="665ba-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="665ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="665ba-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="665ba-126">Request body</span></span>
<span data-ttu-id="665ba-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="665ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="665ba-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="665ba-128">Response</span></span>

<span data-ttu-id="665ba-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AnonymousIpRiskEvent](../resources/anonymousipriskevent.md) den Wert der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="665ba-129">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="665ba-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="665ba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="665ba-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="665ba-131">Request</span></span>
<span data-ttu-id="665ba-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="665ba-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="665ba-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="665ba-133">Response</span></span>
<span data-ttu-id="665ba-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="665ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "ipAddress": null,
  "location": null,
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "AnonymousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/anonymousipriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
