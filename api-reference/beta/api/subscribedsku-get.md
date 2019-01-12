---
title: subscribedSku abrufen
description: Mit dieser API können Sie ein bestimmtes kommerzielles Abonnement abrufen, das eine Organisation erworben hat.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b2d03605060445a351ce0f355caffe49fd029a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960889"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="f345c-103">subscribedSku abrufen</span><span class="sxs-lookup"><span data-stu-id="f345c-103">Get subscribedSku</span></span>

> <span data-ttu-id="f345c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f345c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f345c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f345c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f345c-106">Mit dieser API können Sie ein bestimmtes kommerzielles Abonnement abrufen, das eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="f345c-106">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="f345c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f345c-107">Permissions</span></span>
<span data-ttu-id="f345c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f345c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f345c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f345c-110">Permission type</span></span>      | <span data-ttu-id="f345c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f345c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f345c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f345c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f345c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f345c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f345c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f345c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f345c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f345c-115">Not supported.</span></span>    |
|<span data-ttu-id="f345c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f345c-116">Application</span></span> | <span data-ttu-id="f345c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f345c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f345c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f345c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f345c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f345c-119">Optional query parameters</span></span>
<span data-ttu-id="f345c-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f345c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f345c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f345c-121">Request headers</span></span>
| <span data-ttu-id="f345c-122">Name</span><span class="sxs-lookup"><span data-stu-id="f345c-122">Name</span></span>       | <span data-ttu-id="f345c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f345c-123">Type</span></span> | <span data-ttu-id="f345c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f345c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f345c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f345c-125">Authorization</span></span>  | <span data-ttu-id="f345c-126">string</span><span class="sxs-lookup"><span data-stu-id="f345c-126">string</span></span>  | <span data-ttu-id="f345c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f345c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f345c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f345c-129">Request body</span></span>
<span data-ttu-id="f345c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f345c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f345c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f345c-131">Response</span></span>

<span data-ttu-id="f345c-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscribedSku](../resources/subscribedsku.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f345c-132">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f345c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f345c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f345c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f345c-134">Request</span></span>
<span data-ttu-id="f345c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f345c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="f345c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f345c-136">Response</span></span>
<span data-ttu-id="f345c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f345c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 450

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
