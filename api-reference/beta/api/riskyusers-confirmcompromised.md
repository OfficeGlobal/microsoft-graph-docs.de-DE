---
title: Bestätigen der riskyUsers kompromittiert
description: Bestätigen Sie ein riskyUsers-Objekt als kompromittiert.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 9ae07bf8d1d4a41764aa145a9c7508da339d7ce2
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013124"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="2b1e6-103">Bestätigen der riskyUsers kompromittiert</span><span class="sxs-lookup"><span data-stu-id="2b1e6-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="2b1e6-104">**Hinweis:** Die riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="2b1e6-105">Bestätigen Sie ein [riskyUsers](../resources/riskyuser.md) -Objekt als kompromittiert.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-105">Confirm a [riskyUsers](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="2b1e6-106">Dadurch wird die Risikostufe des Zielbenutzers auf hoch festgelegt.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b1e6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b1e6-107">Permissions</span></span>
<span data-ttu-id="2b1e6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b1e6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b1e6-110">Permission type</span></span>      | <span data-ttu-id="2b1e6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b1e6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b1e6-113">IdentityRiskyUser. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="2b1e6-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b1e6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b1e6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b1e6-115">Not supported.</span></span>    |
|<span data-ttu-id="2b1e6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b1e6-116">Application</span></span> | <span data-ttu-id="2b1e6-117">IdentityRiskyUser. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="2b1e6-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b1e6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b1e6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="2b1e6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b1e6-119">Request headers</span></span>
| <span data-ttu-id="2b1e6-120">Name</span><span class="sxs-lookup"><span data-stu-id="2b1e6-120">Name</span></span>      |<span data-ttu-id="2b1e6-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b1e6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b1e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b1e6-122">Authorization</span></span>  | <span data-ttu-id="2b1e6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b1e6-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2b1e6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b1e6-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b1e6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b1e6-128">Request body</span></span>
<span data-ttu-id="2b1e6-129">Geben Sie die Benutzer-IDs an, die im Anforderungstext geschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="2b1e6-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b1e6-130">Response</span></span>

<span data-ttu-id="2b1e6-131">Bei erfolgreicher Ausführung gibt die Methode den `204 No Content` Antwortcode zurück.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-131">If successful, this method returns a `204 No Content` response code</span></span>
## <a name="example"></a><span data-ttu-id="2b1e6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b1e6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b1e6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b1e6-133">Request</span></span>
<span data-ttu-id="2b1e6-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised


Request Body
{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="2b1e6-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b1e6-135">Response</span></span>
<span data-ttu-id="2b1e6-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b1e6-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
