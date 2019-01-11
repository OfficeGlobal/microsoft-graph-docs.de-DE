---
title: Liste leakedCredentialsRiskEvents
description: Abrufen einer Liste von Leakedcredentialsriskevent-Objekten.
localization_priority: Normal
ms.openlocfilehash: 695499c2db07f108e1f7dd762a97ce95629cca42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857435"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="7f512-103">Liste leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="7f512-103">List leakedCredentialsRiskEvents</span></span>

> <span data-ttu-id="7f512-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f512-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f512-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f512-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f512-106">Abrufen einer Liste von Leakedcredentialsriskevent-Objekten.</span><span class="sxs-lookup"><span data-stu-id="7f512-106">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f512-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f512-107">Permissions</span></span>
<span data-ttu-id="7f512-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f512-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f512-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f512-110">Permission type</span></span>      | <span data-ttu-id="7f512-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f512-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f512-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f512-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f512-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f512-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="7f512-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f512-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f512-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f512-115">Not supported.</span></span>    |
|<span data-ttu-id="7f512-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f512-116">Application</span></span> | <span data-ttu-id="7f512-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f512-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f512-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f512-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="7f512-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f512-119">Request headers</span></span>
| <span data-ttu-id="7f512-120">Name</span><span class="sxs-lookup"><span data-stu-id="7f512-120">Name</span></span>      |<span data-ttu-id="7f512-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f512-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f512-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f512-122">Authorization</span></span>  | <span data-ttu-id="7f512-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f512-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f512-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7f512-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7f512-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7f512-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f512-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f512-128">Request body</span></span>
<span data-ttu-id="7f512-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f512-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f512-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f512-130">Response</span></span>

<span data-ttu-id="7f512-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [LeakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) .</span><span class="sxs-lookup"><span data-stu-id="7f512-131">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f512-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f512-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f512-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f512-133">Request</span></span>
<span data-ttu-id="7f512-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f512-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="7f512-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f512-135">Response</span></span>
<span data-ttu-id="7f512-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f512-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value":
  [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "active",
      "riskLevel": "high",
      "riskType": "LeakedCredentialsRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
