---
title: Benutzer auflisten
description: Dient zum Abrufen einer Liste von Benutzerobjekten. Diese Benutzerobjekte enthalten schulungsspezifische Eigenschaften.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c3614815dd2d43f0b1c43a2ad90eeca73a4782c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982470"
---
# <a name="list-users"></a><span data-ttu-id="8cb8e-104">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="8cb8e-104">List users</span></span>

<span data-ttu-id="8cb8e-105">Dient zum Abrufen einer Liste von Benutzerobjekten.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="8cb8e-106">Diese Benutzerobjekte enthalten schulungsspezifische Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cb8e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8cb8e-107">Permissions</span></span>
<span data-ttu-id="8cb8e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cb8e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb8e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8cb8e-110">Permission type</span></span>      | <span data-ttu-id="8cb8e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8cb8e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cb8e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8cb8e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8cb8e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8cb8e-113">Not supported.</span></span>  |
|<span data-ttu-id="8cb8e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8cb8e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8cb8e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8cb8e-115">Not supported.</span></span>  |
|<span data-ttu-id="8cb8e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8cb8e-116">Application</span></span> | <span data-ttu-id="8cb8e-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb8e-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8cb8e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8cb8e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cb8e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8cb8e-119">Optional query parameters</span></span>
<span data-ttu-id="8cb8e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cb8e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8cb8e-121">Request headers</span></span>
| <span data-ttu-id="8cb8e-122">Header</span><span class="sxs-lookup"><span data-stu-id="8cb8e-122">Header</span></span>       | <span data-ttu-id="8cb8e-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8cb8e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8cb8e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb8e-124">Authorization</span></span>  | <span data-ttu-id="8cb8e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cb8e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8cb8e-127">Request body</span></span>
<span data-ttu-id="8cb8e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8cb8e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8cb8e-129">Response</span></span>
<span data-ttu-id="8cb8e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationUser](../resources/educationuser.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cb8e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8cb8e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cb8e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8cb8e-132">Request</span></span>
<span data-ttu-id="8cb8e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="8cb8e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8cb8e-134">Response</span></span>
<span data-ttu-id="8cb8e-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8cb8e-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8cb8e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
