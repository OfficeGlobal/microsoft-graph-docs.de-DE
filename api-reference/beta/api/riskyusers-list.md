---
title: Liste riskyUsers
description: Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 5c0c0557a5cd84312ef9d6381d8cf3018ab8ce7d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640938"
---
# <a name="list-riskyusers"></a><span data-ttu-id="595ce-103">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="595ce-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="595ce-104">Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="595ce-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="595ce-105">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="595ce-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="595ce-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="595ce-106">Permissions</span></span>
<span data-ttu-id="595ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="595ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="595ce-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="595ce-109">Permission type</span></span>      | <span data-ttu-id="595ce-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="595ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="595ce-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="595ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="595ce-112">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="595ce-112">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="595ce-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="595ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="595ce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="595ce-114">Not supported.</span></span>    |
|<span data-ttu-id="595ce-115">Application</span><span class="sxs-lookup"><span data-stu-id="595ce-115">Application</span></span> | <span data-ttu-id="595ce-116">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="595ce-116">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="595ce-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="595ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="595ce-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="595ce-118">Optional query parameters</span></span>
<span data-ttu-id="595ce-119">Diese Methode unterstützt `$filter` Antwort auf die Abfrage anpassen.</span><span class="sxs-lookup"><span data-stu-id="595ce-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="595ce-120">Siehe das Beispiel weiter unten in diesem Thema.</span><span class="sxs-lookup"><span data-stu-id="595ce-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="595ce-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="595ce-121">Request headers</span></span>
| <span data-ttu-id="595ce-122">Name</span><span class="sxs-lookup"><span data-stu-id="595ce-122">Name</span></span>      |<span data-ttu-id="595ce-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="595ce-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="595ce-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="595ce-124">Authorization</span></span>  | <span data-ttu-id="595ce-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="595ce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="595ce-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="595ce-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="595ce-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="595ce-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="595ce-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="595ce-130">Request body</span></span>
<span data-ttu-id="595ce-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="595ce-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="595ce-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="595ce-132">Response</span></span>

<span data-ttu-id="595ce-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [IdentityRiskEvent](../resources/identityriskevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="595ce-133">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="595ce-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="595ce-134">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="595ce-135">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="595ce-135">Request 1</span></span>
<span data-ttu-id="595ce-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="595ce-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="595ce-137">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="595ce-137">Response 1</span></span>
<span data-ttu-id="595ce-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="595ce-138">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="595ce-139">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="595ce-139">Request 2</span></span>
<span data-ttu-id="595ce-140">Das folgende Beispiel zeigt, wie Sie `$filter` Abrufen der Auflistung der RiskyUser, deren aggregierte Risiko Ebene Mittel ist.</span><span class="sxs-lookup"><span data-stu-id="595ce-140">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="595ce-141">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="595ce-141">Response 2</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
