---
title: EducationSchool abrufen
description: Abrufen der Eigenschaften und Beziehungen des Schulobjekts.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fdd53873322bb9d5f56b2414dd23dee2e88cf9c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946399"
---
# <a name="get-educationschool"></a><span data-ttu-id="ed7f0-103">EducationSchool abrufen</span><span class="sxs-lookup"><span data-stu-id="ed7f0-103">Get educationSchool</span></span>

> <span data-ttu-id="ed7f0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed7f0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed7f0-106">Abrufen der Eigenschaften und Beziehungen des Schulobjekts.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-106">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed7f0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed7f0-107">Permissions</span></span>
<span data-ttu-id="ed7f0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed7f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed7f0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed7f0-110">Permission type</span></span>      | <span data-ttu-id="ed7f0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed7f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed7f0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed7f0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed7f0-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ed7f0-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="ed7f0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed7f0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ed7f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed7f0-115">Not supported.</span></span>  |
|<span data-ttu-id="ed7f0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed7f0-116">Application</span></span> | <span data-ttu-id="ed7f0-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed7f0-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ed7f0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed7f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed7f0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ed7f0-119">Optional query parameters</span></span>
<span data-ttu-id="ed7f0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed7f0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed7f0-121">Request headers</span></span>
| <span data-ttu-id="ed7f0-122">Header</span><span class="sxs-lookup"><span data-stu-id="ed7f0-122">Header</span></span>       | <span data-ttu-id="ed7f0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ed7f0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed7f0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed7f0-124">Authorization</span></span>  | <span data-ttu-id="ed7f0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed7f0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed7f0-127">Request body</span></span>
<span data-ttu-id="ed7f0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ed7f0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed7f0-129">Response</span></span>
<span data-ttu-id="ed7f0-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-130">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed7f0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed7f0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed7f0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed7f0-132">Request</span></span>
<span data-ttu-id="ed7f0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10001
```
##### <a name="response"></a><span data-ttu-id="ed7f0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed7f0-134">Response</span></span>
<span data-ttu-id="ed7f0-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ed7f0-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ed7f0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
