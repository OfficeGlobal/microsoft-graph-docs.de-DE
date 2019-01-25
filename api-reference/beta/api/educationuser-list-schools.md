---
title: Schulen auflisten
description: Dient zum Abrufen einer Liste von Schulen für einen Benutzer.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 594a38d82de173d3a6a93607fdac61cca60e7cac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508566"
---
# <a name="list-schools"></a><span data-ttu-id="a02b9-103">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="a02b9-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a02b9-104">Dient zum Abrufen einer Liste von Schulen für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="a02b9-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="a02b9-105">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="a02b9-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="a02b9-106">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="a02b9-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="a02b9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a02b9-107">Permissions</span></span>
<span data-ttu-id="a02b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a02b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a02b9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a02b9-110">Permission type</span></span>      | <span data-ttu-id="a02b9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a02b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a02b9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a02b9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a02b9-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a02b9-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a02b9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a02b9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a02b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a02b9-115">Not supported.</span></span>  |
|<span data-ttu-id="a02b9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a02b9-116">Application</span></span> | <span data-ttu-id="a02b9-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a02b9-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a02b9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a02b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a02b9-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a02b9-119">Optional query parameters</span></span>
<span data-ttu-id="a02b9-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a02b9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a02b9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a02b9-121">Request headers</span></span>
| <span data-ttu-id="a02b9-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a02b9-122">Header</span></span>       | <span data-ttu-id="a02b9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a02b9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a02b9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a02b9-124">Authorization</span></span>  | <span data-ttu-id="a02b9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a02b9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a02b9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a02b9-127">Request body</span></span>
<span data-ttu-id="a02b9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a02b9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a02b9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a02b9-129">Response</span></span>
<span data-ttu-id="a02b9-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationSchool](../resources/educationschool.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a02b9-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a02b9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a02b9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a02b9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a02b9-132">Request</span></span>
<span data-ttu-id="a02b9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a02b9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="a02b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a02b9-134">Response</span></span>
<span data-ttu-id="a02b9-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a02b9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a02b9-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a02b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
