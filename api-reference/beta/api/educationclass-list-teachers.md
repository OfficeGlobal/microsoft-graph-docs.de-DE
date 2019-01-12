---
title: Lehrer auflisten
description: Abrufen einer Liste der Lehrer für eine Klasse. Delegierte Token müssen zum Abrufen der Liste der Lehrer Mitglieder der Klasse sein.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 871090596ec83e9af90a37e8afc6f4b8f67faed5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960511"
---
# <a name="list-teachers"></a><span data-ttu-id="c8142-104">Lehrer auflisten</span><span class="sxs-lookup"><span data-stu-id="c8142-104">List teachers</span></span>

> <span data-ttu-id="c8142-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8142-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8142-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8142-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8142-107">Abrufen einer Liste der Lehrer für eine Klasse.</span><span class="sxs-lookup"><span data-stu-id="c8142-107">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="c8142-108">Delegierte Token müssen zum Abrufen der Liste der Lehrer Mitglieder der Klasse sein.</span><span class="sxs-lookup"><span data-stu-id="c8142-108">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8142-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8142-109">Permissions</span></span>
<span data-ttu-id="c8142-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8142-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8142-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8142-112">Permission type</span></span>      | <span data-ttu-id="c8142-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8142-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8142-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8142-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c8142-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c8142-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c8142-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8142-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="c8142-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8142-117">Not supported.</span></span>  |
|<span data-ttu-id="c8142-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8142-118">Application</span></span> | <span data-ttu-id="c8142-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8142-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c8142-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8142-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8142-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c8142-121">Optional query parameters</span></span>
<span data-ttu-id="c8142-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8142-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8142-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8142-123">Request headers</span></span>
| <span data-ttu-id="c8142-124">Header</span><span class="sxs-lookup"><span data-stu-id="c8142-124">Header</span></span>       | <span data-ttu-id="c8142-125">Wert</span><span class="sxs-lookup"><span data-stu-id="c8142-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8142-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8142-126">Authorization</span></span>  | <span data-ttu-id="c8142-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8142-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8142-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8142-129">Request body</span></span>
<span data-ttu-id="c8142-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8142-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c8142-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8142-131">Response</span></span>
<span data-ttu-id="c8142-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationUser](../resources/educationuser.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8142-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8142-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8142-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8142-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8142-134">Request</span></span>
<span data-ttu-id="c8142-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8142-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023/teachers
```
##### <a name="response"></a><span data-ttu-id="c8142-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8142-136">Response</span></span>
<span data-ttu-id="c8142-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8142-137">The following is an example of the response.</span></span> 

><span data-ttu-id="c8142-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c8142-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
