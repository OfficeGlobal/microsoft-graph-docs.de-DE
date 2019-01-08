---
title: Organisation abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.
ms.openlocfilehash: 842fe286a83b41f44c64b4c80d0095c20170f0d4
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748394"
---
# <a name="get-organization"></a><span data-ttu-id="b13f3-103">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="b13f3-103">Get organization</span></span>

<span data-ttu-id="b13f3-104">Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.</span><span class="sxs-lookup"><span data-stu-id="b13f3-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b13f3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b13f3-105">Permissions</span></span>

<span data-ttu-id="b13f3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b13f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b13f3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b13f3-108">Permission type</span></span>      | <span data-ttu-id="b13f3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b13f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b13f3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b13f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b13f3-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b13f3-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="b13f3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b13f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b13f3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b13f3-113">Not supported.</span></span>    |
|<span data-ttu-id="b13f3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b13f3-114">Application</span></span> | <span data-ttu-id="b13f3-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b13f3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="b13f3-116">Hinweis: Anwendungen, denen die User.Read-Berechtigung gewährt wurde, können nur die *id*-, *displayName*- und *verifiedDomains*-Eigenschaften der Organisation lesen.</span><span class="sxs-lookup"><span data-stu-id="b13f3-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="b13f3-117">Alle anderen Eigenschaften geben `null`-Werte zurück.</span><span class="sxs-lookup"><span data-stu-id="b13f3-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="b13f3-118">Verwenden Sie zum Lesen aller Eigenschaften Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="b13f3-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="b13f3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b13f3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b13f3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b13f3-120">Optional query parameters</span></span>

<span data-ttu-id="b13f3-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b13f3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b13f3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b13f3-122">Request headers</span></span>

| <span data-ttu-id="b13f3-123">Name</span><span class="sxs-lookup"><span data-stu-id="b13f3-123">Name</span></span>       | <span data-ttu-id="b13f3-124">Typ</span><span class="sxs-lookup"><span data-stu-id="b13f3-124">Type</span></span> | <span data-ttu-id="b13f3-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b13f3-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b13f3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b13f3-126">Authorization</span></span>  | <span data-ttu-id="b13f3-127">string</span><span class="sxs-lookup"><span data-stu-id="b13f3-127">string</span></span>  | <span data-ttu-id="b13f3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b13f3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b13f3-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b13f3-130">Request body</span></span>

<span data-ttu-id="b13f3-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b13f3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b13f3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b13f3-132">Response</span></span>

<span data-ttu-id="b13f3-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von [einem Organisationsobjekt im Antworttext](../resources/organization.md) .</span><span class="sxs-lookup"><span data-stu-id="b13f3-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b13f3-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b13f3-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b13f3-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b13f3-135">Request</span></span>

<span data-ttu-id="b13f3-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b13f3-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```

##### <a name="response"></a><span data-ttu-id="b13f3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b13f3-137">Response</span></span>

<span data-ttu-id="b13f3-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b13f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
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
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->