---
title: Abrufen der Vereinbarung
description: Rufen Sie die Eigenschaften und die Beziehungen eines Vereinbarung-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: da36b6cb2d12c92d4bf12ec2ce4836f5bbc5efe1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517127"
---
# <a name="get-agreement"></a><span data-ttu-id="65e18-103">Abrufen der Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="65e18-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65e18-104">Rufen Sie die Eigenschaften und die Beziehungen eines [Vereinbarung](../resources/agreement.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="65e18-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="65e18-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65e18-105">Permissions</span></span>
<span data-ttu-id="65e18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65e18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e18-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65e18-108">Permission type</span></span>                        | <span data-ttu-id="65e18-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65e18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="65e18-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65e18-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="65e18-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="65e18-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="65e18-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65e18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65e18-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65e18-113">Not supported.</span></span> |
|<span data-ttu-id="65e18-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65e18-114">Application</span></span>                            | <span data-ttu-id="65e18-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65e18-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65e18-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65e18-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="65e18-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65e18-117">Request headers</span></span>
| <span data-ttu-id="65e18-118">Name</span><span class="sxs-lookup"><span data-stu-id="65e18-118">Name</span></span>         | <span data-ttu-id="65e18-119">Typ</span><span class="sxs-lookup"><span data-stu-id="65e18-119">Type</span></span>        | <span data-ttu-id="65e18-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65e18-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="65e18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e18-121">Authorization</span></span> | <span data-ttu-id="65e18-122">string</span><span class="sxs-lookup"><span data-stu-id="65e18-122">string</span></span> | <span data-ttu-id="65e18-123">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="65e18-123">Bearer \{token\}.</span></span> <span data-ttu-id="65e18-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65e18-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65e18-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65e18-125">Request body</span></span>
<span data-ttu-id="65e18-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="65e18-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="65e18-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="65e18-127">Response</span></span>
<span data-ttu-id="65e18-128">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortobjekt Code und [Vereinbarung](../resources/agreement.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="65e18-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65e18-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65e18-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65e18-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65e18-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="65e18-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="65e18-131">Response</span></span>
><span data-ttu-id="65e18-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="65e18-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
