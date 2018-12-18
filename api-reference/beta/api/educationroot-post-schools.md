---
title: EducationSchool erstellen
description: Erstellt eine Bildungseinrichtung.
author: mmast-msft
ms.openlocfilehash: 5be5d144f7e4a1887c9fde6196009963d9ce9893
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356126"
---
# <a name="create-educationschool"></a><span data-ttu-id="211e2-103">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="211e2-103">Create educationSchool</span></span>

> <span data-ttu-id="211e2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="211e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="211e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="211e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="211e2-106">Erstellt eine Bildungseinrichtung.</span><span class="sxs-lookup"><span data-stu-id="211e2-106">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="211e2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="211e2-107">Permissions</span></span>
<span data-ttu-id="211e2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="211e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="211e2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="211e2-110">Permission type</span></span>      | <span data-ttu-id="211e2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="211e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="211e2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="211e2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="211e2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="211e2-113">Not supported.</span></span>  |
|<span data-ttu-id="211e2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="211e2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="211e2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="211e2-115">Not supported.</span></span>  |
|<span data-ttu-id="211e2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="211e2-116">Application</span></span> | <span data-ttu-id="211e2-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="211e2-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="211e2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="211e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="211e2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="211e2-119">Request headers</span></span>
| <span data-ttu-id="211e2-120">Header</span><span class="sxs-lookup"><span data-stu-id="211e2-120">Header</span></span>       | <span data-ttu-id="211e2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="211e2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="211e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="211e2-122">Authorization</span></span>  | <span data-ttu-id="211e2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="211e2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="211e2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="211e2-125">Content-Type</span></span>  | <span data-ttu-id="211e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="211e2-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="211e2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="211e2-127">Request body</span></span>
<span data-ttu-id="211e2-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationSchool](../resources/educationschool.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="211e2-128">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="211e2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="211e2-129">Response</span></span>
<span data-ttu-id="211e2-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="211e2-130">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="211e2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="211e2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="211e2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="211e2-132">Request</span></span>
<span data-ttu-id="211e2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="211e2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="211e2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="211e2-134">Response</span></span>
<span data-ttu-id="211e2-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="211e2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="211e2-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="211e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
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
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->