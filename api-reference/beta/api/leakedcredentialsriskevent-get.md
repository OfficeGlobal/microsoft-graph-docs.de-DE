---
title: Abrufen von leakedCredentialsRiskEvent
description: Rufen Sie die Eigenschaften und die Beziehungen eines Leakedcredentialsriskevent-Objekts ab.
ms.openlocfilehash: a3d259f785d2c8d6717f4dfe90ba04aeb454a1bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065521"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="62746-103">Abrufen von leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="62746-103">Get leakedCredentialsRiskEvent</span></span>

> <span data-ttu-id="62746-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="62746-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62746-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62746-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62746-106">Rufen Sie die Eigenschaften und die Beziehungen eines Leakedcredentialsriskevent-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="62746-106">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="62746-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="62746-107">Permissions</span></span>
<span data-ttu-id="62746-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62746-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62746-110">Permission type</span></span>      | <span data-ttu-id="62746-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62746-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62746-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62746-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62746-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="62746-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="62746-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62746-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62746-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62746-115">Not supported.</span></span>    |
|<span data-ttu-id="62746-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62746-116">Application</span></span> | <span data-ttu-id="62746-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="62746-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62746-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62746-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="62746-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62746-119">Request headers</span></span>
| <span data-ttu-id="62746-120">Name</span><span class="sxs-lookup"><span data-stu-id="62746-120">Name</span></span>      |<span data-ttu-id="62746-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62746-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62746-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62746-122">Authorization</span></span>  | <span data-ttu-id="62746-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="62746-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62746-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="62746-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="62746-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="62746-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62746-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62746-128">Request body</span></span>
<span data-ttu-id="62746-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="62746-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62746-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="62746-130">Response</span></span>

<span data-ttu-id="62746-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [LeakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="62746-131">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="62746-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62746-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62746-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62746-133">Request</span></span>
<span data-ttu-id="62746-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62746-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="62746-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="62746-135">Response</span></span>
<span data-ttu-id="62746-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62746-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
