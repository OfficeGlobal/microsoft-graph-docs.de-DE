---
title: Organisation auflisten
description: Mit dieser API können Sie eine Liste von Organisationsobjekten abrufen.
localization_priority: Normal
ms.openlocfilehash: 7087ea0ef7e3885334b33d53416d5e4b6fc750a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882796"
---
# <a name="list-organization"></a><span data-ttu-id="52628-103">Organisation auflisten</span><span class="sxs-lookup"><span data-stu-id="52628-103">List organization</span></span>

> <span data-ttu-id="52628-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="52628-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52628-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52628-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52628-106">Mit dieser API können Sie eine Liste von Organisationsobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="52628-106">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="52628-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="52628-107">Permissions</span></span>
<span data-ttu-id="52628-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52628-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52628-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52628-110">Permission type</span></span>      | <span data-ttu-id="52628-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52628-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52628-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52628-112">Delegated (work or school account)</span></span> | <span data-ttu-id="52628-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52628-113">Not supported.</span></span>    |
|<span data-ttu-id="52628-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52628-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52628-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52628-115">Not supported.</span></span>    |
|<span data-ttu-id="52628-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52628-116">Application</span></span> | <span data-ttu-id="52628-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52628-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52628-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52628-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52628-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="52628-119">Optional query parameters</span></span>
<span data-ttu-id="52628-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="52628-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52628-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52628-121">Request headers</span></span>
| <span data-ttu-id="52628-122">Name</span><span class="sxs-lookup"><span data-stu-id="52628-122">Name</span></span>       | <span data-ttu-id="52628-123">Typ</span><span class="sxs-lookup"><span data-stu-id="52628-123">Type</span></span> | <span data-ttu-id="52628-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52628-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52628-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="52628-125">Authorization</span></span>  | <span data-ttu-id="52628-126">string</span><span class="sxs-lookup"><span data-stu-id="52628-126">string</span></span>  | <span data-ttu-id="52628-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52628-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52628-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52628-129">Request body</span></span>
<span data-ttu-id="52628-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="52628-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52628-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="52628-131">Response</span></span>

<span data-ttu-id="52628-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [organization](../resources/organization.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52628-132">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52628-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52628-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52628-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52628-134">Request</span></span>
<span data-ttu-id="52628-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52628-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="52628-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="52628-136">Response</span></span>
<span data-ttu-id="52628-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52628-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
