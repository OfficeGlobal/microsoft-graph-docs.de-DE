---
title: Organisation auflisten
description: Mit dieser API können Sie eine Liste von Organisationsobjekten abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9dd1489714c4de87f0072ef0498c5acdf008d5ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938825"
---
# <a name="list-organization"></a><span data-ttu-id="8fecc-103">Organisation auflisten</span><span class="sxs-lookup"><span data-stu-id="8fecc-103">List organization</span></span>

> <span data-ttu-id="8fecc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8fecc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fecc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fecc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fecc-106">Mit dieser API können Sie eine Liste von Organisationsobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="8fecc-106">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8fecc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8fecc-107">Permissions</span></span>
<span data-ttu-id="8fecc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fecc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fecc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fecc-110">Permission type</span></span>      | <span data-ttu-id="8fecc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fecc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fecc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fecc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8fecc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fecc-113">Not supported.</span></span>    |
|<span data-ttu-id="8fecc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fecc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fecc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fecc-115">Not supported.</span></span>    |
|<span data-ttu-id="8fecc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fecc-116">Application</span></span> | <span data-ttu-id="8fecc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fecc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fecc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fecc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8fecc-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8fecc-119">Optional query parameters</span></span>
<span data-ttu-id="8fecc-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8fecc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8fecc-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fecc-121">Request headers</span></span>
| <span data-ttu-id="8fecc-122">Name</span><span class="sxs-lookup"><span data-stu-id="8fecc-122">Name</span></span>       | <span data-ttu-id="8fecc-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8fecc-123">Type</span></span> | <span data-ttu-id="8fecc-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fecc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8fecc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fecc-125">Authorization</span></span>  | <span data-ttu-id="8fecc-126">string</span><span class="sxs-lookup"><span data-stu-id="8fecc-126">string</span></span>  | <span data-ttu-id="8fecc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fecc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fecc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fecc-129">Request body</span></span>
<span data-ttu-id="8fecc-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8fecc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fecc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fecc-131">Response</span></span>

<span data-ttu-id="8fecc-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [organization](../resources/organization.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fecc-132">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8fecc-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fecc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fecc-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fecc-134">Request</span></span>
<span data-ttu-id="8fecc-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fecc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="8fecc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fecc-136">Response</span></span>
<span data-ttu-id="8fecc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fecc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
