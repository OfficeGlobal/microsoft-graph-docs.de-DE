---
title: Abrufen von riskyUsers
description: Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 586e76cd57e720741c6a63bc00374cd0973a1cf3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642345"
---
# <a name="get-riskyusers"></a><span data-ttu-id="3f937-103">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3f937-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f937-104">Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="3f937-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="3f937-105">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3f937-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f937-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3f937-106">Permissions</span></span>
<span data-ttu-id="3f937-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f937-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f937-109">Permission type</span></span>      | <span data-ttu-id="3f937-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f937-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f937-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f937-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f937-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f937-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="3f937-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f937-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f937-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f937-114">Not supported.</span></span>    |
|<span data-ttu-id="3f937-115">Application</span><span class="sxs-lookup"><span data-stu-id="3f937-115">Application</span></span> | <span data-ttu-id="3f937-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f937-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f937-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f937-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="3f937-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f937-118">Request headers</span></span>
| <span data-ttu-id="3f937-119">Name</span><span class="sxs-lookup"><span data-stu-id="3f937-119">Name</span></span>      |<span data-ttu-id="3f937-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f937-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f937-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f937-121">Authorization</span></span>  | <span data-ttu-id="3f937-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3f937-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f937-124">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3f937-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3f937-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3f937-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f937-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3f937-127">Request body</span></span>
<span data-ttu-id="3f937-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3f937-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f937-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f937-129">Response</span></span>

<span data-ttu-id="3f937-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [RiskyUser](../resources/riskyuser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3f937-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f937-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f937-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f937-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f937-132">Request</span></span>
<span data-ttu-id="3f937-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f937-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="3f937-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f937-134">Response</span></span>
<span data-ttu-id="3f937-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f937-135">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
