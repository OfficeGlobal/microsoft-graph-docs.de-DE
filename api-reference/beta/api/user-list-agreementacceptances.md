---
title: Liste agreementAcceptances
description: Abrufen einer Liste der AgreementAcceptance-Objekte des Benutzers an.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22babc13c3b1db4cf143a35ab2119e97c43c822b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517869"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="4d234-103">Liste agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="4d234-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d234-104">Abrufen einer Liste der [AgreementAcceptance](../resources/agreementacceptance.md) -Objekte des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="4d234-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d234-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d234-105">Permissions</span></span>
<span data-ttu-id="4d234-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d234-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d234-108">Permission type</span></span>                        | <span data-ttu-id="4d234-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d234-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d234-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d234-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d234-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="4d234-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="4d234-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d234-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d234-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d234-113">Not supported.</span></span> |
|<span data-ttu-id="4d234-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d234-114">Application</span></span>                            | <span data-ttu-id="4d234-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d234-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d234-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d234-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="4d234-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d234-117">Request headers</span></span>
| <span data-ttu-id="4d234-118">Name</span><span class="sxs-lookup"><span data-stu-id="4d234-118">Name</span></span>      |<span data-ttu-id="4d234-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d234-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d234-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d234-120">Authorization</span></span> | <span data-ttu-id="4d234-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4d234-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d234-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d234-122">Request body</span></span>
<span data-ttu-id="4d234-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d234-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4d234-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d234-124">Response</span></span>
<span data-ttu-id="4d234-125">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AgreementAcceptance](../resources/agreementacceptance.md) .</span><span class="sxs-lookup"><span data-stu-id="4d234-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d234-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d234-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d234-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d234-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="4d234-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d234-128">Response</span></span>
><span data-ttu-id="4d234-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4d234-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
