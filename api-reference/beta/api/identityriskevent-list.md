---
title: Liste identityRiskEvents
description: Abrufen einer Liste von Identityriskevent-Objekten.
author: cloudhandler
ms.openlocfilehash: ee730b2da90cd1d458bd3e3ad4c432db93fa4cea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302779"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="484ad-103">Liste identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="484ad-103">List identityRiskEvents</span></span>

> <span data-ttu-id="484ad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="484ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="484ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="484ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="484ad-106">Abrufen einer Liste von Identityriskevent-Objekten.</span><span class="sxs-lookup"><span data-stu-id="484ad-106">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="484ad-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="484ad-107">Permissions</span></span>
<span data-ttu-id="484ad-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="484ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="484ad-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="484ad-110">Permission type</span></span>      | <span data-ttu-id="484ad-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="484ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="484ad-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="484ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="484ad-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="484ad-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="484ad-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="484ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="484ad-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="484ad-115">Not supported.</span></span>    |
|<span data-ttu-id="484ad-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="484ad-116">Application</span></span> | <span data-ttu-id="484ad-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="484ad-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="484ad-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="484ad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="484ad-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="484ad-119">Request headers</span></span>
| <span data-ttu-id="484ad-120">Name</span><span class="sxs-lookup"><span data-stu-id="484ad-120">Name</span></span>      |<span data-ttu-id="484ad-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="484ad-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="484ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="484ad-122">Authorization</span></span>  | <span data-ttu-id="484ad-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="484ad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="484ad-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="484ad-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="484ad-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="484ad-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="484ad-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="484ad-128">Request body</span></span>
<span data-ttu-id="484ad-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="484ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="484ad-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="484ad-130">Response</span></span>

<span data-ttu-id="484ad-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [IdentityRiskEvent](../resources/identityriskevent.md) .</span><span class="sxs-lookup"><span data-stu-id="484ad-131">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="484ad-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="484ad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="484ad-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="484ad-133">Request</span></span>
<span data-ttu-id="484ad-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="484ad-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="484ad-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="484ad-135">Response</span></span>
<span data-ttu-id="484ad-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="484ad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
