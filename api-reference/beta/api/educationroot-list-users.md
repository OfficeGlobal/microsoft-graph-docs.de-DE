---
title: Benutzer auflisten
description: Dient zum Abrufen einer Liste von Benutzerobjekten. Diese Benutzerobjekte enthalten schulungsspezifische Eigenschaften.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 761725dae02839721fbc710aecd30d4d8d5b03d3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524968"
---
# <a name="list-users"></a><span data-ttu-id="251da-104">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="251da-104">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="251da-105">Dient zum Abrufen einer Liste von Benutzerobjekten.</span><span class="sxs-lookup"><span data-stu-id="251da-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="251da-106">Diese Benutzerobjekte enthalten schulungsspezifische Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="251da-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="251da-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="251da-107">Permissions</span></span>
<span data-ttu-id="251da-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="251da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="251da-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="251da-110">Permission type</span></span>      | <span data-ttu-id="251da-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="251da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="251da-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="251da-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="251da-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="251da-113">Not supported.</span></span>  |
|<span data-ttu-id="251da-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="251da-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="251da-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="251da-115">Not supported.</span></span>  |
|<span data-ttu-id="251da-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="251da-116">Application</span></span> | <span data-ttu-id="251da-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="251da-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="251da-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="251da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="251da-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="251da-119">Optional query parameters</span></span>
<span data-ttu-id="251da-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="251da-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="251da-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="251da-121">Request headers</span></span>
| <span data-ttu-id="251da-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="251da-122">Header</span></span>       | <span data-ttu-id="251da-123">Wert</span><span class="sxs-lookup"><span data-stu-id="251da-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="251da-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="251da-124">Authorization</span></span>  | <span data-ttu-id="251da-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="251da-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="251da-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="251da-127">Request body</span></span>
<span data-ttu-id="251da-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="251da-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="251da-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="251da-129">Response</span></span>
<span data-ttu-id="251da-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationUser](../resources/educationuser.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="251da-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="251da-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="251da-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="251da-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="251da-132">Request</span></span>
<span data-ttu-id="251da-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="251da-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/users
```
##### <a name="response"></a><span data-ttu-id="251da-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="251da-134">Response</span></span>
<span data-ttu-id="251da-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="251da-135">The following is an example of the response.</span></span> 

><span data-ttu-id="251da-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="251da-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationroot-list-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
