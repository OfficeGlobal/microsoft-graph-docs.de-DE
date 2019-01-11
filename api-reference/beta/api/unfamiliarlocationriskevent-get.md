---
title: Abrufen von unfamiliarLocationRiskEvent
description: Rufen Sie die Eigenschaften und die Beziehungen eines Unfamiliarlocationriskevent-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: d58fc2c5b2c84ae0b43bbc2b83345d6bc6bff700
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827939"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="3e272-103">Abrufen von unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="3e272-103">Get unfamiliarLocationRiskEvent</span></span>

> <span data-ttu-id="3e272-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e272-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e272-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e272-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e272-106">Rufen Sie die Eigenschaften und die Beziehungen eines Unfamiliarlocationriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="3e272-106">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e272-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e272-107">Permissions</span></span>
<span data-ttu-id="3e272-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e272-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e272-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e272-110">Permission type</span></span>      | <span data-ttu-id="3e272-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e272-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e272-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e272-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e272-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e272-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3e272-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e272-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e272-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e272-115">Not supported.</span></span>    |
|<span data-ttu-id="3e272-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e272-116">Application</span></span> | <span data-ttu-id="3e272-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e272-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e272-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e272-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3e272-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e272-119">Request headers</span></span>
| <span data-ttu-id="3e272-120">Name</span><span class="sxs-lookup"><span data-stu-id="3e272-120">Name</span></span>      |<span data-ttu-id="3e272-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e272-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e272-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e272-122">Authorization</span></span>  | <span data-ttu-id="3e272-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e272-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e272-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3e272-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e272-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3e272-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e272-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e272-128">Request body</span></span>
<span data-ttu-id="3e272-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3e272-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e272-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e272-130">Response</span></span>

<span data-ttu-id="3e272-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [UnfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3e272-131">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e272-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e272-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e272-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e272-133">Request</span></span>
<span data-ttu-id="3e272-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e272-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="3e272-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e272-135">Response</span></span>
<span data-ttu-id="3e272-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e272-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
