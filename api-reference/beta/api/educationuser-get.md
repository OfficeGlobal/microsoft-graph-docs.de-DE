---
title: EducationUser abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines Benutzers.
ms.openlocfilehash: e40b4bfea7daa1d6df1b5d06b9a8e67407647b28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058015"
---
# <a name="get-educationuser"></a><span data-ttu-id="cd3b5-103">EducationUser abrufen</span><span class="sxs-lookup"><span data-stu-id="cd3b5-103">Get educationUser</span></span>

> <span data-ttu-id="cd3b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd3b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd3b5-106">Dient zum Abrufen der Eigenschaften und Beziehungen eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-106">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd3b5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd3b5-107">Permissions</span></span>
<span data-ttu-id="cd3b5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd3b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd3b5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd3b5-110">Permission type</span></span>      | <span data-ttu-id="cd3b5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd3b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd3b5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd3b5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cd3b5-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="cd3b5-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="cd3b5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd3b5-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cd3b5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd3b5-115">Not supported.</span></span>  |
|<span data-ttu-id="cd3b5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd3b5-116">Application</span></span> | <span data-ttu-id="cd3b5-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd3b5-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="cd3b5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd3b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd3b5-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd3b5-119">Optional query parameters</span></span>
<span data-ttu-id="cd3b5-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd3b5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd3b5-121">Request headers</span></span>
| <span data-ttu-id="cd3b5-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd3b5-122">Header</span></span>       | <span data-ttu-id="cd3b5-123">Wert</span><span class="sxs-lookup"><span data-stu-id="cd3b5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd3b5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd3b5-124">Authorization</span></span>  | <span data-ttu-id="cd3b5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd3b5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd3b5-127">Request body</span></span>
<span data-ttu-id="cd3b5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cd3b5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd3b5-129">Response</span></span>
<span data-ttu-id="cd3b5-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-130">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd3b5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd3b5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd3b5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd3b5-132">Request</span></span>
<span data-ttu-id="cd3b5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="cd3b5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd3b5-134">Response</span></span>
<span data-ttu-id="cd3b5-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-135">The following is an example of the response.</span></span> 

><span data-ttu-id="cd3b5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cd3b5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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