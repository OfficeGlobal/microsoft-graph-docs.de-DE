---
title: subscribedSkus auflisten
description: Mit dieser API können Sie eine Liste aller kommerziellen Abonnements abrufen, die eine Organisation erworben hat.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 38b76629f995aa44de2f05cfe20d8ac24e24acd9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515146"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="e259f-103">subscribedSkus auflisten</span><span class="sxs-lookup"><span data-stu-id="e259f-103">List subscribedSkus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e259f-104">Mit dieser API können Sie eine Liste aller kommerziellen Abonnements abrufen, die eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="e259f-104">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="e259f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e259f-105">Permissions</span></span>
<span data-ttu-id="e259f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e259f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e259f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e259f-108">Permission type</span></span>      | <span data-ttu-id="e259f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e259f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e259f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e259f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e259f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e259f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e259f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e259f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e259f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e259f-113">Not supported.</span></span>    |
|<span data-ttu-id="e259f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e259f-114">Application</span></span> | <span data-ttu-id="e259f-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e259f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e259f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e259f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e259f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e259f-117">Optional query parameters</span></span>
<span data-ttu-id="e259f-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e259f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e259f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e259f-119">Request headers</span></span>
| <span data-ttu-id="e259f-120">Name</span><span class="sxs-lookup"><span data-stu-id="e259f-120">Name</span></span>       | <span data-ttu-id="e259f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e259f-121">Type</span></span> | <span data-ttu-id="e259f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e259f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e259f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e259f-123">Authorization</span></span>  | <span data-ttu-id="e259f-124">string</span><span class="sxs-lookup"><span data-stu-id="e259f-124">string</span></span>  | <span data-ttu-id="e259f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e259f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e259f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e259f-127">Request body</span></span>
<span data-ttu-id="e259f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e259f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e259f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e259f-129">Response</span></span>

<span data-ttu-id="e259f-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ChartSeries](../resources/subscribedsku.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e259f-130">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e259f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e259f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e259f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e259f-132">Request</span></span>
<span data-ttu-id="e259f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e259f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus
```
##### <a name="response"></a><span data-ttu-id="e259f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e259f-134">Response</span></span>
<span data-ttu-id="e259f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e259f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
  "value": [
    {
      "capabilityStatus": "capabilityStatus-value",
      "consumedUnits": 99,
      "prepaidUnits": {
        "enabled": 99,
        "suspended": 99,
        "warning": 99
      },
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscribedsku-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
