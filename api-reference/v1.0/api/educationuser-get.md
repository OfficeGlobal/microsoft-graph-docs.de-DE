---
title: EducationUser abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines Benutzers.
author: mmast-msft
ms.openlocfilehash: df7b2de211b8950350e9d4418c053d0cc8b7b90b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337114"
---
# <a name="get-educationuser"></a><span data-ttu-id="3f7ab-103">EducationUser abrufen</span><span class="sxs-lookup"><span data-stu-id="3f7ab-103">Get educationUser</span></span>

<span data-ttu-id="3f7ab-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-104">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f7ab-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3f7ab-105">Permissions</span></span>
<span data-ttu-id="3f7ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f7ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f7ab-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f7ab-108">Permission type</span></span>      | <span data-ttu-id="3f7ab-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f7ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f7ab-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f7ab-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3f7ab-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3f7ab-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3f7ab-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f7ab-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3f7ab-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f7ab-113">Not supported.</span></span>  |
|<span data-ttu-id="3f7ab-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3f7ab-114">Application</span></span> | <span data-ttu-id="3f7ab-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f7ab-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="3f7ab-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f7ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f7ab-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3f7ab-117">Optional query parameters</span></span>
<span data-ttu-id="3f7ab-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f7ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f7ab-119">Request headers</span></span>
| <span data-ttu-id="3f7ab-120">Header</span><span class="sxs-lookup"><span data-stu-id="3f7ab-120">Header</span></span>       | <span data-ttu-id="3f7ab-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3f7ab-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f7ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f7ab-122">Authorization</span></span>  | <span data-ttu-id="3f7ab-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f7ab-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3f7ab-125">Request body</span></span>
<span data-ttu-id="3f7ab-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3f7ab-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f7ab-127">Response</span></span>
<span data-ttu-id="3f7ab-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-128">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f7ab-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f7ab-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f7ab-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f7ab-130">Request</span></span>
<span data-ttu-id="3f7ab-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="3f7ab-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f7ab-132">Response</span></span>
<span data-ttu-id="3f7ab-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-133">The following is an example of the response.</span></span> 

><span data-ttu-id="3f7ab-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3f7ab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->