---
title: Mitglieder auflisten
description: 'Abrufen der Lehrer und Kursteilnehmer für eine Klasse. Hinweis: Wenn das delegierte Token verwendet wird, werden Mitglieder nur anderen Mitgliedern der Klasse angezeigt.'
ms.openlocfilehash: 8543f429fec359fe91275c8636e2eded686c9db5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019406"
---
# <a name="list-members"></a><span data-ttu-id="2b508-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="2b508-104">List members</span></span>

<span data-ttu-id="2b508-105">Abrufen der Lehrer und Kursteilnehmer für eine Klasse.</span><span class="sxs-lookup"><span data-stu-id="2b508-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="2b508-106">Hinweis: Wenn das delegierte Token verwendet wird, werden Mitglieder nur anderen Mitgliedern der Klasse angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2b508-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b508-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b508-107">Permissions</span></span>
<span data-ttu-id="2b508-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b508-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b508-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b508-110">Permission type</span></span>      | <span data-ttu-id="2b508-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b508-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b508-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b508-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b508-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2b508-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2b508-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b508-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2b508-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b508-115">Not supported</span></span>  |
|<span data-ttu-id="2b508-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b508-116">Application</span></span> | <span data-ttu-id="2b508-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="2b508-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2b508-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b508-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b508-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2b508-119">Optional query parameters</span></span>
<span data-ttu-id="2b508-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b508-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b508-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b508-121">Request headers</span></span>
| <span data-ttu-id="2b508-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2b508-122">Header</span></span>       | <span data-ttu-id="2b508-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2b508-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b508-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b508-124">Authorization</span></span>  | <span data-ttu-id="2b508-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b508-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b508-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b508-127">Request body</span></span>
<span data-ttu-id="2b508-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2b508-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2b508-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b508-129">Response</span></span>
<span data-ttu-id="2b508-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationUser](../resources/educationuser.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b508-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b508-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b508-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b508-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b508-132">Request</span></span>
<span data-ttu-id="2b508-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b508-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="2b508-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b508-134">Response</span></span>
<span data-ttu-id="2b508-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b508-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2b508-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2b508-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->