---
title: subscribedSku abrufen
description: Mit dieser API können Sie ein bestimmtes kommerzielles Abonnement abrufen, das eine Organisation erworben hat.
ms.openlocfilehash: cf7d8ef7aef8eaabdc30c02c9bf8e71478017823
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017473"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="05af8-103">subscribedSku abrufen</span><span class="sxs-lookup"><span data-stu-id="05af8-103">Get subscribedSku</span></span>
<span data-ttu-id="05af8-104">Mit dieser API können Sie ein bestimmtes kommerzielles Abonnement abrufen, das eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="05af8-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="05af8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="05af8-105">Permissions</span></span>
<span data-ttu-id="05af8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05af8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="05af8-108">Permission type</span></span>      | <span data-ttu-id="05af8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="05af8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05af8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="05af8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05af8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05af8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05af8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="05af8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05af8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05af8-113">Not supported.</span></span>    |
|<span data-ttu-id="05af8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="05af8-114">Application</span></span> | <span data-ttu-id="05af8-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05af8-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05af8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="05af8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05af8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="05af8-117">Optional query parameters</span></span>
<span data-ttu-id="05af8-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="05af8-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="05af8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="05af8-119">Request headers</span></span>
| <span data-ttu-id="05af8-120">Name</span><span class="sxs-lookup"><span data-stu-id="05af8-120">Name</span></span>       | <span data-ttu-id="05af8-121">Typ</span><span class="sxs-lookup"><span data-stu-id="05af8-121">Type</span></span> | <span data-ttu-id="05af8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05af8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="05af8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05af8-123">Authorization</span></span>  | <span data-ttu-id="05af8-124">string</span><span class="sxs-lookup"><span data-stu-id="05af8-124">string</span></span>  | <span data-ttu-id="05af8-p102">Bearer &lt;token&gt;. *Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="05af8-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="05af8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="05af8-127">Request body</span></span>
<span data-ttu-id="05af8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="05af8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05af8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="05af8-129">Response</span></span>

<span data-ttu-id="05af8-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscribedSku](../resources/subscribedsku.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05af8-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05af8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="05af8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05af8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="05af8-132">Request</span></span>
<span data-ttu-id="05af8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="05af8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="05af8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="05af8-134">Response</span></span>
<span data-ttu-id="05af8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05af8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus/$entity",
    "capabilityStatus": "Enabled",
    "consumedUnits": 14,
    "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
    "prepaidUnits": {
        "enabled": 25,
        "suspended": 0,
        "warning": 0
    },
    "servicePlans": [
        {
            "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
            "servicePlanName": "ADALLOM_S_O365",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->