---
title: Abrufen von identityRiskEvent
description: Rufen Sie die Eigenschaften und Beziehungen des Identityriskevent-Objekts ab.
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: aaec2759ee3dd6b1e4b12a77124560c5b0985c42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818032"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="08adf-103">Abrufen von identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="08adf-103">Get identityRiskEvent</span></span>

> <span data-ttu-id="08adf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08adf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08adf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08adf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08adf-106">Rufen Sie die Eigenschaften und Beziehungen des Identityriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="08adf-106">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="08adf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="08adf-107">Permissions</span></span>
<span data-ttu-id="08adf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08adf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08adf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08adf-110">Permission type</span></span>      | <span data-ttu-id="08adf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08adf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08adf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08adf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08adf-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="08adf-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="08adf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08adf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08adf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08adf-115">Not supported.</span></span>    |
|<span data-ttu-id="08adf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08adf-116">Application</span></span> | <span data-ttu-id="08adf-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="08adf-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08adf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08adf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="08adf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08adf-119">Request headers</span></span>
| <span data-ttu-id="08adf-120">Name</span><span class="sxs-lookup"><span data-stu-id="08adf-120">Name</span></span>      |<span data-ttu-id="08adf-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08adf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08adf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08adf-122">Authorization</span></span>  | <span data-ttu-id="08adf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08adf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08adf-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="08adf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="08adf-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="08adf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08adf-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08adf-128">Request body</span></span>
<span data-ttu-id="08adf-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="08adf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08adf-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="08adf-130">Response</span></span>

<span data-ttu-id="08adf-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [IdentityRiskEvent](../resources/identityriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="08adf-131">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08adf-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08adf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08adf-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08adf-133">Request</span></span>
<span data-ttu-id="08adf-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08adf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="08adf-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="08adf-135">Response</span></span>
<span data-ttu-id="08adf-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08adf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
