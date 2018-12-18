---
title: Schulen auflisten
description: Abrufen einer Liste von Schulen, in denen der Kurs unterrichtet wird.
author: mmast-msft
ms.openlocfilehash: 8de8e443780797044d451505de0a5e4f72fe34b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316541"
---
# <a name="list-schools"></a><span data-ttu-id="68d19-103">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="68d19-103">List schools</span></span>

> <span data-ttu-id="68d19-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68d19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68d19-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68d19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68d19-106">Abrufen einer Liste von Schulen, in denen der Kurs unterrichtet wird.</span><span class="sxs-lookup"><span data-stu-id="68d19-106">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="68d19-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68d19-107">Permissions</span></span>
<span data-ttu-id="68d19-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68d19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68d19-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68d19-110">Permission type</span></span>      | <span data-ttu-id="68d19-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68d19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68d19-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68d19-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="68d19-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="68d19-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="68d19-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68d19-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="68d19-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68d19-115">Not supported</span></span>  |
|<span data-ttu-id="68d19-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68d19-116">Application</span></span> | <span data-ttu-id="68d19-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68d19-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="68d19-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68d19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68d19-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68d19-119">Optional query parameters</span></span>
<span data-ttu-id="68d19-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68d19-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68d19-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68d19-121">Request headers</span></span>
| <span data-ttu-id="68d19-122">Header</span><span class="sxs-lookup"><span data-stu-id="68d19-122">Header</span></span>       | <span data-ttu-id="68d19-123">Wert</span><span class="sxs-lookup"><span data-stu-id="68d19-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68d19-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="68d19-124">Authorization</span></span>  | <span data-ttu-id="68d19-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68d19-p103">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="68d19-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68d19-127">Request body</span></span>
<span data-ttu-id="68d19-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68d19-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="68d19-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="68d19-129">Response</span></span>
<span data-ttu-id="68d19-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationSchool](../resources/educationschool.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68d19-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68d19-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68d19-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68d19-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68d19-132">Request</span></span>
<span data-ttu-id="68d19-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68d19-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```
##### <a name="response"></a><span data-ttu-id="68d19-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="68d19-134">Response</span></span>
<span data-ttu-id="68d19-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68d19-135">The following is an example of the response.</span></span> 

><span data-ttu-id="68d19-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="68d19-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10002",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
