---
title: EducationUser erstellen
description: Erstellen eines neuen Benutzers.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 29785bdc2a3afe8bce1521f7321da53eda66ff0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947358"
---
# <a name="create-educationuser"></a><span data-ttu-id="127fc-103">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="127fc-103">Create educationUser</span></span>

<span data-ttu-id="127fc-104">Erstellen eines neuen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="127fc-104">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="127fc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="127fc-105">Permissions</span></span>
<span data-ttu-id="127fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127fc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="127fc-108">Permission type</span></span>      | <span data-ttu-id="127fc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="127fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="127fc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="127fc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="127fc-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="127fc-111">Not supported.</span></span>  |
|<span data-ttu-id="127fc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="127fc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="127fc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="127fc-113">Not supported.</span></span>  |
|<span data-ttu-id="127fc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="127fc-114">Application</span></span> | <span data-ttu-id="127fc-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127fc-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="127fc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="127fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="127fc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="127fc-117">Request headers</span></span>
| <span data-ttu-id="127fc-118">Header</span><span class="sxs-lookup"><span data-stu-id="127fc-118">Header</span></span>       | <span data-ttu-id="127fc-119">Wert</span><span class="sxs-lookup"><span data-stu-id="127fc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="127fc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="127fc-120">Authorization</span></span>  | <span data-ttu-id="127fc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="127fc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="127fc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="127fc-123">Content-Type</span></span>  | <span data-ttu-id="127fc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="127fc-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="127fc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="127fc-125">Request body</span></span>
<span data-ttu-id="127fc-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="127fc-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="127fc-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="127fc-127">Response</span></span>
<span data-ttu-id="127fc-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="127fc-128">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="127fc-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="127fc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="127fc-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="127fc-130">Request</span></span>
<span data-ttu-id="127fc-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="127fc-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/users
Content-type: application/json
Content-length: 508

{
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
```

##### <a name="response"></a><span data-ttu-id="127fc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="127fc-132">Response</span></span>
<span data-ttu-id="127fc-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="127fc-133">The following is an example of the response.</span></span> 

><span data-ttu-id="127fc-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="127fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
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
      "id": "14012",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
