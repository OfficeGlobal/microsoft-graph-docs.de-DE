---
title: Abrufen von riskyUsers
description: Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.
ms.openlocfilehash: f0a6ac24bf66184d0547e9284f5a35b84b9358b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059132"
---
# <a name="get-riskyusers"></a><span data-ttu-id="ecb76-103">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ecb76-103">Get riskyUsers</span></span>

> <span data-ttu-id="ecb76-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ecb76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecb76-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ecb76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecb76-106">Rufen Sie die Eigenschaften und die Beziehungen eines **RiskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="ecb76-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ecb76-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ecb76-107">Permissions</span></span>
<span data-ttu-id="ecb76-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb76-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ecb76-110">Permission type</span></span>      | <span data-ttu-id="ecb76-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ecb76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecb76-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ecb76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ecb76-113">IdentityrRskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecb76-113">IdentityrRskyUser.Read.All</span></span>    |
|<span data-ttu-id="ecb76-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ecb76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb76-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecb76-115">Not supported.</span></span>    |
|<span data-ttu-id="ecb76-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecb76-116">Application</span></span> | <span data-ttu-id="ecb76-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecb76-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecb76-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecb76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="ecb76-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ecb76-119">Request headers</span></span>
| <span data-ttu-id="ecb76-120">Name</span><span class="sxs-lookup"><span data-stu-id="ecb76-120">Name</span></span>      |<span data-ttu-id="ecb76-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecb76-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecb76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecb76-122">Authorization</span></span>  | <span data-ttu-id="ecb76-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ecb76-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ecb76-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ecb76-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ecb76-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ecb76-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb76-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ecb76-128">Request body</span></span>
<span data-ttu-id="ecb76-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ecb76-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb76-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecb76-130">Response</span></span>

<span data-ttu-id="ecb76-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [RiskyUser](../resources/riskyuser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ecb76-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ecb76-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecb76-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ecb76-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecb76-133">Request</span></span>
<span data-ttu-id="ecb76-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ecb76-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="ecb76-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecb76-135">Response</span></span>
<span data-ttu-id="ecb76-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ecb76-136">Here is an example of the response.</span></span>
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
