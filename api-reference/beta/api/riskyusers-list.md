---
title: Liste riskyUsers
description: Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.
ms.openlocfilehash: 152171ff098bb58e8cbb247ca687841e77594ead
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066130"
---
# <a name="list-riskyusers"></a><span data-ttu-id="bf386-103">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="bf386-103">List riskyUsers</span></span>

> <span data-ttu-id="bf386-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bf386-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf386-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf386-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf386-106">Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="bf386-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf386-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bf386-107">Permissions</span></span>
<span data-ttu-id="bf386-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf386-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf386-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf386-110">Permission type</span></span>      | <span data-ttu-id="bf386-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf386-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf386-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf386-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf386-113">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf386-113">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="bf386-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf386-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf386-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf386-115">Not supported.</span></span>    |
|<span data-ttu-id="bf386-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf386-116">Application</span></span> | <span data-ttu-id="bf386-117">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf386-117">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf386-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf386-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bf386-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bf386-119">Optional query parameters</span></span>
<span data-ttu-id="bf386-120">Diese Methode unterstützt `$filter` Antwort auf die Abfrage anpassen.</span><span class="sxs-lookup"><span data-stu-id="bf386-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="bf386-121">Siehe das Beispiel weiter unten in diesem Thema.</span><span class="sxs-lookup"><span data-stu-id="bf386-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="bf386-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf386-122">Request headers</span></span>
| <span data-ttu-id="bf386-123">Name</span><span class="sxs-lookup"><span data-stu-id="bf386-123">Name</span></span>      |<span data-ttu-id="bf386-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf386-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf386-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf386-125">Authorization</span></span>  | <span data-ttu-id="bf386-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf386-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf386-128">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="bf386-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf386-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="bf386-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf386-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf386-131">Request body</span></span>
<span data-ttu-id="bf386-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bf386-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf386-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf386-133">Response</span></span>

<span data-ttu-id="bf386-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [IdentityRiskEvent](../resources/identityriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bf386-134">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf386-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf386-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="bf386-136">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="bf386-136">Request 1</span></span>
<span data-ttu-id="bf386-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf386-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="bf386-138">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="bf386-138">Response 1</span></span>
<span data-ttu-id="bf386-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bf386-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
##### <a name="request-2"></a><span data-ttu-id="bf386-140">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="bf386-140">Request 2</span></span>
<span data-ttu-id="bf386-141">Das folgende Beispiel zeigt, wie Sie `$filter` Abrufen der Auflistung der RiskyUser, deren aggregierte Risiko Ebene Mittel ist.</span><span class="sxs-lookup"><span data-stu-id="bf386-141">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="bf386-142">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="bf386-142">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
      "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com",
      }
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
