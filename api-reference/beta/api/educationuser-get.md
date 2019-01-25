---
title: EducationUser abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines Benutzers.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0d2f20099de7083ce5dd09dbe98893c680490820
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530139"
---
# <a name="get-educationuser"></a><span data-ttu-id="5b47e-103">EducationUser abrufen</span><span class="sxs-lookup"><span data-stu-id="5b47e-103">Get educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b47e-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5b47e-104">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b47e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b47e-105">Permissions</span></span>
<span data-ttu-id="5b47e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b47e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b47e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b47e-108">Permission type</span></span>      | <span data-ttu-id="5b47e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b47e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b47e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b47e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5b47e-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5b47e-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="5b47e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b47e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5b47e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b47e-113">Not supported.</span></span>  |
|<span data-ttu-id="5b47e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b47e-114">Application</span></span> | <span data-ttu-id="5b47e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b47e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="5b47e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b47e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b47e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5b47e-117">Optional query parameters</span></span>
<span data-ttu-id="5b47e-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b47e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b47e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b47e-119">Request headers</span></span>
| <span data-ttu-id="5b47e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b47e-120">Header</span></span>       | <span data-ttu-id="5b47e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5b47e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b47e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b47e-122">Authorization</span></span>  | <span data-ttu-id="5b47e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b47e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b47e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b47e-125">Request body</span></span>
<span data-ttu-id="5b47e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b47e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5b47e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b47e-127">Response</span></span>
<span data-ttu-id="5b47e-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b47e-128">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b47e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b47e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b47e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b47e-130">Request</span></span>
<span data-ttu-id="5b47e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b47e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="5b47e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b47e-132">Response</span></span>
<span data-ttu-id="5b47e-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b47e-133">The following is an example of the response.</span></span> 

><span data-ttu-id="5b47e-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5b47e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
