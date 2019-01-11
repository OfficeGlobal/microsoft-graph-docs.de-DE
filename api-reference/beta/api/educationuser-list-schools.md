---
title: Schulen auflisten
description: Dient zum Abrufen einer Liste von Schulen für einen Benutzer.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: dfe2e48d0246e30d93bebd019c4b7f81ae788e66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883500"
---
# <a name="list-schools"></a><span data-ttu-id="1803d-103">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="1803d-103">List schools</span></span>

> <span data-ttu-id="1803d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1803d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1803d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1803d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1803d-106">Dient zum Abrufen einer Liste von Schulen für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="1803d-106">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="1803d-107">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="1803d-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="1803d-108">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="1803d-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="1803d-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1803d-109">Permissions</span></span>
<span data-ttu-id="1803d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1803d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1803d-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1803d-112">Permission type</span></span>      | <span data-ttu-id="1803d-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1803d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1803d-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1803d-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="1803d-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1803d-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="1803d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1803d-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1803d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1803d-117">Not supported.</span></span>  |
|<span data-ttu-id="1803d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1803d-118">Application</span></span> | <span data-ttu-id="1803d-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1803d-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1803d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1803d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1803d-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1803d-121">Optional query parameters</span></span>
<span data-ttu-id="1803d-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1803d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1803d-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1803d-123">Request headers</span></span>
| <span data-ttu-id="1803d-124">Header</span><span class="sxs-lookup"><span data-stu-id="1803d-124">Header</span></span>       | <span data-ttu-id="1803d-125">Wert</span><span class="sxs-lookup"><span data-stu-id="1803d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1803d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1803d-126">Authorization</span></span>  | <span data-ttu-id="1803d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1803d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1803d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1803d-129">Request body</span></span>
<span data-ttu-id="1803d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1803d-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1803d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1803d-131">Response</span></span>
<span data-ttu-id="1803d-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationSchool](../resources/educationschool.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1803d-132">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1803d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1803d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1803d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1803d-134">Request</span></span>
<span data-ttu-id="1803d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1803d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="1803d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="1803d-136">Response</span></span>
<span data-ttu-id="1803d-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1803d-137">The following is an example of the response.</span></span> 

><span data-ttu-id="1803d-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1803d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
