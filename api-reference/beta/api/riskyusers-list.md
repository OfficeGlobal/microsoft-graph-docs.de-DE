---
title: Liste riskyUsers
description: Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: f2763a963d27bbb0a2fc1515a36aec199bd29f19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953441"
---
# <a name="list-riskyusers"></a><span data-ttu-id="e4fa1-103">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e4fa1-103">List riskyUsers</span></span>

> <span data-ttu-id="e4fa1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4fa1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4fa1-106">Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="e4fa1-107">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4fa1-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4fa1-108">Permissions</span></span>
<span data-ttu-id="e4fa1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4fa1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4fa1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4fa1-111">Permission type</span></span>      | <span data-ttu-id="e4fa1-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4fa1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4fa1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4fa1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e4fa1-114">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4fa1-114">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="e4fa1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4fa1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4fa1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4fa1-116">Not supported.</span></span>    |
|<span data-ttu-id="e4fa1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4fa1-117">Application</span></span> | <span data-ttu-id="e4fa1-118">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4fa1-118">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4fa1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4fa1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4fa1-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e4fa1-120">Optional query parameters</span></span>
<span data-ttu-id="e4fa1-121">Diese Methode unterstützt `$filter` Antwort auf die Abfrage anpassen.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-121">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="e4fa1-122">Siehe das Beispiel weiter unten in diesem Thema.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-122">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e4fa1-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4fa1-123">Request headers</span></span>
| <span data-ttu-id="e4fa1-124">Name</span><span class="sxs-lookup"><span data-stu-id="e4fa1-124">Name</span></span>      |<span data-ttu-id="e4fa1-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4fa1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4fa1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4fa1-126">Authorization</span></span>  | <span data-ttu-id="e4fa1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4fa1-129">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e4fa1-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4fa1-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4fa1-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4fa1-132">Request body</span></span>
<span data-ttu-id="e4fa1-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4fa1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4fa1-134">Response</span></span>

<span data-ttu-id="e4fa1-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [IdentityRiskEvent](../resources/identityriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-135">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4fa1-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4fa1-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e4fa1-137">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="e4fa1-137">Request 1</span></span>
<span data-ttu-id="e4fa1-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="e4fa1-139">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="e4fa1-139">Response 1</span></span>
<span data-ttu-id="e4fa1-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-140">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="e4fa1-141">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="e4fa1-141">Request 2</span></span>
<span data-ttu-id="e4fa1-142">Das folgende Beispiel zeigt, wie Sie `$filter` Abrufen der Auflistung der RiskyUser, deren aggregierte Risiko Ebene Mittel ist.</span><span class="sxs-lookup"><span data-stu-id="e4fa1-142">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="e4fa1-143">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="e4fa1-143">Response 2</span></span>
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
