---
title: Liste suspiciousIpRiskEvents
description: Abrufen einer Liste von Suspiciousipriskevent-Objekten.
ms.openlocfilehash: fe6d14b4f1c7fc1d65b6293de156a63ed2bd15a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065637"
---
# <a name="list-suspiciousipriskevents"></a><span data-ttu-id="8f5fb-103">Liste suspiciousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="8f5fb-103">List suspiciousIpRiskEvents</span></span>

> <span data-ttu-id="8f5fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f5fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f5fb-106">Abrufen einer Liste von Suspiciousipriskevent-Objekten.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-106">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f5fb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8f5fb-107">Permissions</span></span>
<span data-ttu-id="8f5fb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f5fb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f5fb-110">Permission type</span></span>      | <span data-ttu-id="8f5fb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f5fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f5fb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f5fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f5fb-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f5fb-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="8f5fb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f5fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f5fb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f5fb-115">Not supported.</span></span>    |
|<span data-ttu-id="8f5fb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f5fb-116">Application</span></span> | <span data-ttu-id="8f5fb-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f5fb-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f5fb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f5fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="8f5fb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f5fb-119">Request headers</span></span>
| <span data-ttu-id="8f5fb-120">Name</span><span class="sxs-lookup"><span data-stu-id="8f5fb-120">Name</span></span>      |<span data-ttu-id="8f5fb-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f5fb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f5fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f5fb-122">Authorization</span></span>  | <span data-ttu-id="8f5fb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f5fb-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8f5fb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f5fb-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f5fb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f5fb-128">Request body</span></span>
<span data-ttu-id="8f5fb-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f5fb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f5fb-130">Response</span></span>

<span data-ttu-id="8f5fb-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [SuspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) .</span><span class="sxs-lookup"><span data-stu-id="8f5fb-131">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f5fb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f5fb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f5fb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f5fb-133">Request</span></span>
<span data-ttu-id="8f5fb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="8f5fb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f5fb-135">Response</span></span>
<span data-ttu-id="8f5fb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f5fb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
