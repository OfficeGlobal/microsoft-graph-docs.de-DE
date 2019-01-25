---
title: Liste suspiciousIpRiskEvents
description: Abrufen einer Liste von Suspiciousipriskevent-Objekten.
localization_priority: Normal
ms.openlocfilehash: 1caad773d401367b93bece5d30191a5c98b7b935
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513802"
---
# <a name="list-suspiciousipriskevents"></a><span data-ttu-id="b9eca-103">Liste suspiciousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="b9eca-103">List suspiciousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9eca-104">Abrufen einer Liste von Suspiciousipriskevent-Objekten.</span><span class="sxs-lookup"><span data-stu-id="b9eca-104">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9eca-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9eca-105">Permissions</span></span>
<span data-ttu-id="b9eca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9eca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9eca-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9eca-108">Permission type</span></span>      | <span data-ttu-id="b9eca-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9eca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9eca-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9eca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9eca-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9eca-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="b9eca-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9eca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9eca-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9eca-113">Not supported.</span></span>    |
|<span data-ttu-id="b9eca-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9eca-114">Application</span></span> | <span data-ttu-id="b9eca-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9eca-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9eca-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9eca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="b9eca-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9eca-117">Request headers</span></span>
| <span data-ttu-id="b9eca-118">Name</span><span class="sxs-lookup"><span data-stu-id="b9eca-118">Name</span></span>      |<span data-ttu-id="b9eca-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9eca-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9eca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9eca-120">Authorization</span></span>  | <span data-ttu-id="b9eca-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9eca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9eca-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b9eca-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9eca-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b9eca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9eca-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9eca-126">Request body</span></span>
<span data-ttu-id="b9eca-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9eca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9eca-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9eca-128">Response</span></span>

<span data-ttu-id="b9eca-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [SuspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) .</span><span class="sxs-lookup"><span data-stu-id="b9eca-129">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9eca-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9eca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9eca-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9eca-131">Request</span></span>
<span data-ttu-id="b9eca-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9eca-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="b9eca-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9eca-133">Response</span></span>
<span data-ttu-id="b9eca-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9eca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/suspiciousipriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
