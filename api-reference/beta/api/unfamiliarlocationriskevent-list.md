---
title: Liste unfamiliarLocationRiskEvents
description: Abrufen einer Liste von Unfamiliarlocationriskevent-Objekten.
ms.openlocfilehash: 2a0decd6ecf700f2679bc905a7a64c261b7a532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063249"
---
# <a name="list-unfamiliarlocationriskevents"></a><span data-ttu-id="52779-103">Liste unfamiliarLocationRiskEvents</span><span class="sxs-lookup"><span data-stu-id="52779-103">List unfamiliarLocationRiskEvents</span></span>

> <span data-ttu-id="52779-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="52779-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52779-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52779-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52779-106">Abrufen einer Liste von Unfamiliarlocationriskevent-Objekten.</span><span class="sxs-lookup"><span data-stu-id="52779-106">Retrieve a list of unfamiliarlocationriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="52779-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="52779-107">Permissions</span></span>
<span data-ttu-id="52779-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52779-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52779-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52779-110">Permission type</span></span>      | <span data-ttu-id="52779-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52779-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52779-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52779-112">Delegated (work or school account)</span></span> | <span data-ttu-id="52779-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="52779-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="52779-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52779-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52779-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52779-115">Not supported.</span></span>    |
|<span data-ttu-id="52779-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52779-116">Application</span></span> | <span data-ttu-id="52779-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="52779-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52779-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52779-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="52779-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52779-119">Request headers</span></span>
| <span data-ttu-id="52779-120">Name</span><span class="sxs-lookup"><span data-stu-id="52779-120">Name</span></span>      |<span data-ttu-id="52779-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52779-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52779-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52779-122">Authorization</span></span>  | <span data-ttu-id="52779-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52779-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52779-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="52779-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="52779-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="52779-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52779-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52779-128">Request body</span></span>
<span data-ttu-id="52779-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="52779-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52779-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="52779-130">Response</span></span>

<span data-ttu-id="52779-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [UnfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) .</span><span class="sxs-lookup"><span data-stu-id="52779-131">If successful, this method returns a `200 OK` response code and collection of [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52779-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52779-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52779-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52779-133">Request</span></span>
<span data-ttu-id="52779-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52779-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents
```
##### <a name="response"></a><span data-ttu-id="52779-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="52779-135">Response</span></span>
<span data-ttu-id="52779-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52779-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List unfamiliarLocationRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
