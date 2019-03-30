---
title: RiskyUsers abrufen
description: Ruft die Eigenschaften und Beziehungen eines **riskyUsers** -Objekts ab.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b65135fcd1ad77304b98f18fa595154aee984910
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003713"
---
# <a name="get-riskyusers"></a><span data-ttu-id="b758a-103">RiskyUsers abrufen</span><span class="sxs-lookup"><span data-stu-id="b758a-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b758a-104">Ruft die Eigenschaften und Beziehungen eines **riskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="b758a-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="b758a-105">**Hinweis:** Die Verwendung der riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="b758a-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="b758a-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b758a-106">Permissions</span></span>
<span data-ttu-id="b758a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b758a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b758a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b758a-109">Permission type</span></span>      | <span data-ttu-id="b758a-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b758a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b758a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b758a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b758a-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="b758a-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="b758a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b758a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b758a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b758a-114">Not supported.</span></span>    |
|<span data-ttu-id="b758a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b758a-115">Application</span></span> | <span data-ttu-id="b758a-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="b758a-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b758a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b758a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="b758a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b758a-118">Request headers</span></span>
| <span data-ttu-id="b758a-119">Name</span><span class="sxs-lookup"><span data-stu-id="b758a-119">Name</span></span>      |<span data-ttu-id="b758a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b758a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b758a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b758a-121">Authorization</span></span>  | <span data-ttu-id="b758a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b758a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b758a-124">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b758a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b758a-125">Sitzungs-ID der Arbeitsmappe, die bestimmt, ob Änderungen beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="b758a-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="b758a-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="b758a-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b758a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b758a-127">Request body</span></span>
<span data-ttu-id="b758a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b758a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b758a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b758a-129">Response</span></span>

<span data-ttu-id="b758a-130">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [riskyUser](../resources/riskyUser.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b758a-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b758a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b758a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b758a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b758a-132">Request</span></span>
<span data-ttu-id="b758a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b758a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="b758a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b758a-134">Response</span></span>
<span data-ttu-id="b758a-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b758a-135">Here is an example of the response.</span></span>
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
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

