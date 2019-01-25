---
title: Domänen auflisten
description: Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7cbc4237d7fad61366102a25b65ffd4718c61d62
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512150"
---
# <a name="list-domains"></a><span data-ttu-id="8a96d-103">Domänen auflisten</span><span class="sxs-lookup"><span data-stu-id="8a96d-103">List domains</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a96d-104">Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="8a96d-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a96d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a96d-105">Permissions</span></span>
<span data-ttu-id="8a96d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a96d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a96d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a96d-108">Permission type</span></span>      | <span data-ttu-id="8a96d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a96d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a96d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a96d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a96d-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a96d-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="8a96d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a96d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a96d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a96d-113">Not supported.</span></span>    |
|<span data-ttu-id="8a96d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a96d-114">Application</span></span> | <span data-ttu-id="8a96d-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a96d-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a96d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a96d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a96d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8a96d-117">Optional query parameters</span></span>
<span data-ttu-id="8a96d-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8a96d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a96d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a96d-119">Request headers</span></span>
| <span data-ttu-id="8a96d-120">Name</span><span class="sxs-lookup"><span data-stu-id="8a96d-120">Name</span></span>      |<span data-ttu-id="8a96d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a96d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8a96d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a96d-122">Authorization</span></span>  | <span data-ttu-id="8a96d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a96d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8a96d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8a96d-125">Accept</span></span>         | <span data-ttu-id="8a96d-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="8a96d-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a96d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a96d-127">Request body</span></span>
<span data-ttu-id="8a96d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8a96d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a96d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a96d-129">Response</span></span>

<span data-ttu-id="8a96d-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domain](../resources/domain.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a96d-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a96d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a96d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a96d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a96d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
##### <a name="response"></a><span data-ttu-id="8a96d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a96d-133">Response</span></span>
<span data-ttu-id="8a96d-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a96d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
