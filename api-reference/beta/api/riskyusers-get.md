---
title: Abrufen von riskyUsers
description: Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.
localization_priority: Normal
ms.openlocfilehash: da26be10b5a1aa631bd55f977ead806ed89c1406
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891126"
---
# <a name="get-riskyusers"></a><span data-ttu-id="5b36f-103">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5b36f-103">Get riskyUsers</span></span>

> <span data-ttu-id="5b36f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b36f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b36f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b36f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b36f-106">Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="5b36f-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="5b36f-107">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b36f-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b36f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b36f-108">Permissions</span></span>
<span data-ttu-id="5b36f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b36f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b36f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b36f-111">Permission type</span></span>      | <span data-ttu-id="5b36f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b36f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b36f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b36f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b36f-114">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b36f-114">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="5b36f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b36f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b36f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b36f-116">Not supported.</span></span>    |
|<span data-ttu-id="5b36f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b36f-117">Application</span></span> | <span data-ttu-id="5b36f-118">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b36f-118">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b36f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b36f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="5b36f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b36f-120">Request headers</span></span>
| <span data-ttu-id="5b36f-121">Name</span><span class="sxs-lookup"><span data-stu-id="5b36f-121">Name</span></span>      |<span data-ttu-id="5b36f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b36f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b36f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b36f-123">Authorization</span></span>  | <span data-ttu-id="5b36f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b36f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b36f-126">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5b36f-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="5b36f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5b36f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b36f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b36f-129">Request body</span></span>
<span data-ttu-id="5b36f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b36f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b36f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b36f-131">Response</span></span>

<span data-ttu-id="5b36f-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [RiskyUser](../resources/riskyuser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5b36f-132">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b36f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b36f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b36f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b36f-134">Request</span></span>
<span data-ttu-id="5b36f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b36f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="5b36f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b36f-136">Response</span></span>
<span data-ttu-id="5b36f-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b36f-137">Here is an example of the response.</span></span>
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
