---
title: EducationUser erstellen
description: Erstellen eines neuen Benutzers.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9e9555e91455c841f5f4143def5e77d30d7a121b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946420"
---
# <a name="create-educationuser"></a><span data-ttu-id="2237c-103">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="2237c-103">Create educationUser</span></span>

> <span data-ttu-id="2237c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2237c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2237c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2237c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2237c-106">Erstellen eines neuen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2237c-106">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="2237c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2237c-107">Permissions</span></span>
<span data-ttu-id="2237c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2237c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2237c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2237c-110">Permission type</span></span>      | <span data-ttu-id="2237c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2237c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2237c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2237c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2237c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2237c-113">Not supported.</span></span>  |
|<span data-ttu-id="2237c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2237c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2237c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2237c-115">Not supported.</span></span>  |
|<span data-ttu-id="2237c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2237c-116">Application</span></span> | <span data-ttu-id="2237c-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2237c-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2237c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2237c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="2237c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2237c-119">Request headers</span></span>
| <span data-ttu-id="2237c-120">Header</span><span class="sxs-lookup"><span data-stu-id="2237c-120">Header</span></span>       | <span data-ttu-id="2237c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2237c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2237c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2237c-122">Authorization</span></span>  | <span data-ttu-id="2237c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2237c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2237c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2237c-125">Content-Type</span></span>  | <span data-ttu-id="2237c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2237c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2237c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2237c-127">Request body</span></span>
<span data-ttu-id="2237c-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2237c-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2237c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2237c-129">Response</span></span>
<span data-ttu-id="2237c-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2237c-130">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2237c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2237c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2237c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2237c-132">Request</span></span>
<span data-ttu-id="2237c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2237c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
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

##### <a name="response"></a><span data-ttu-id="2237c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2237c-134">Response</span></span>
<span data-ttu-id="2237c-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2237c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2237c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2237c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
