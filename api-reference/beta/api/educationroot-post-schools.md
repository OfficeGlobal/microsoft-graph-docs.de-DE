---
title: EducationSchool erstellen
description: Erstellt eine Bildungseinrichtung.
ms.openlocfilehash: 2007da0974b42b305c66b617dfe4d6fd5eb0e4c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058360"
---
# <a name="create-educationschool"></a><span data-ttu-id="dd500-103">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="dd500-103">Create educationSchool</span></span>

> <span data-ttu-id="dd500-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd500-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd500-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd500-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd500-106">Erstellt eine Bildungseinrichtung.</span><span class="sxs-lookup"><span data-stu-id="dd500-106">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd500-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd500-107">Permissions</span></span>
<span data-ttu-id="dd500-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd500-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd500-110">Permission type</span></span>      | <span data-ttu-id="dd500-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd500-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd500-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd500-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="dd500-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd500-113">Not supported.</span></span>  |
|<span data-ttu-id="dd500-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd500-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dd500-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd500-115">Not supported.</span></span>  |
|<span data-ttu-id="dd500-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd500-116">Application</span></span> | <span data-ttu-id="dd500-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd500-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dd500-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd500-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="dd500-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd500-119">Request headers</span></span>
| <span data-ttu-id="dd500-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd500-120">Header</span></span>       | <span data-ttu-id="dd500-121">Wert</span><span class="sxs-lookup"><span data-stu-id="dd500-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd500-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd500-122">Authorization</span></span>  | <span data-ttu-id="dd500-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd500-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dd500-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd500-125">Content-Type</span></span>  | <span data-ttu-id="dd500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd500-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd500-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd500-127">Request body</span></span>
<span data-ttu-id="dd500-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationSchool](../resources/educationschool.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="dd500-128">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="dd500-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd500-129">Response</span></span>
<span data-ttu-id="dd500-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd500-130">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd500-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd500-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd500-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd500-132">Request</span></span>
<span data-ttu-id="dd500-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd500-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dd500-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd500-134">Response</span></span>
<span data-ttu-id="dd500-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd500-135">The following is an example of the response.</span></span> 

><span data-ttu-id="dd500-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="dd500-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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