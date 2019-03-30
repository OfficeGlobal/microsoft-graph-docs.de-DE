---
title: RiskyUsers aufListen
description: Ruft die Eigenschaften und Beziehungen eines **riskyUsers** -Objekts ab.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a902daf00f80470e1ac9a83a287eac507d55e171
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003727"
---
# <a name="list-riskyusers"></a><span data-ttu-id="20b9d-103">RiskyUsers aufListen</span><span class="sxs-lookup"><span data-stu-id="20b9d-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20b9d-104">Ruft die Eigenschaften und Beziehungen eines **riskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="20b9d-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="20b9d-105">**Hinweis:** Die Verwendung der riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="20b9d-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="20b9d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="20b9d-106">Permissions</span></span>
<span data-ttu-id="20b9d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b9d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20b9d-109">Permission type</span></span>      | <span data-ttu-id="20b9d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20b9d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20b9d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20b9d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20b9d-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b9d-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="20b9d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20b9d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20b9d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20b9d-114">Not supported.</span></span>    |
|<span data-ttu-id="20b9d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20b9d-115">Application</span></span> | <span data-ttu-id="20b9d-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b9d-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20b9d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20b9d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20b9d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="20b9d-118">Optional query parameters</span></span>
<span data-ttu-id="20b9d-119">Diese Methode unter `$filter` stützt die Anpassung der Abfrageantwort.</span><span class="sxs-lookup"><span data-stu-id="20b9d-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="20b9d-120">Sehen Sie sich das Beispiel weiter unten in diesem Thema an.</span><span class="sxs-lookup"><span data-stu-id="20b9d-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="20b9d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20b9d-121">Request headers</span></span>
| <span data-ttu-id="20b9d-122">Name</span><span class="sxs-lookup"><span data-stu-id="20b9d-122">Name</span></span>      |<span data-ttu-id="20b9d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20b9d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20b9d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="20b9d-124">Authorization</span></span>  | <span data-ttu-id="20b9d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="20b9d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20b9d-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="20b9d-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="20b9d-128">Sitzungs-ID der Arbeitsmappe, die bestimmt, ob Änderungen beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="20b9d-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="20b9d-129">Optional.</span><span class="sxs-lookup"><span data-stu-id="20b9d-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b9d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20b9d-130">Request body</span></span>
<span data-ttu-id="20b9d-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="20b9d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20b9d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="20b9d-132">Response</span></span>

<span data-ttu-id="20b9d-133">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [identityRiskEvent](../resources/identityriskevent.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="20b9d-133">If successful, this method returns a `200 OK` response code and an [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="20b9d-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="20b9d-134">Examples</span></span>
#### <a name="example-1-list-risky-users"></a><span data-ttu-id="20b9d-135">Beispiel 1: aufListen von riskanten Benutzern</span><span class="sxs-lookup"><span data-stu-id="20b9d-135">Example 1: List risky users</span></span>
<span data-ttu-id="20b9d-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20b9d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```

<span data-ttu-id="20b9d-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="20b9d-137">Here is an example of the response.</span></span>
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
  "isProcessing": true,
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
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
#### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="20b9d-138">Beispiel 2: aufListen von riskanten Benutzern und Filtern der Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="20b9d-138">Example 2: List risky users and filter the results</span></span>
<span data-ttu-id="20b9d-139">Das folgende Beispiel zeigt, wie Sie `$filter` die Auflistung von riskyUser abrufen, deren aggregierte Risikostufe Mittel ist.</span><span class="sxs-lookup"><span data-stu-id="20b9d-139">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
<span data-ttu-id="20b9d-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="20b9d-140">Here is an example of the response.</span></span>
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
      "isProcessing": true,
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
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
