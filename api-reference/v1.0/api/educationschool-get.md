---
title: EducationSchool abrufen
description: Abrufen der Eigenschaften und Beziehungen des Schulobjekts.
ms.openlocfilehash: bfa3d680446578e48954f828e6f07fed787e3b95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017400"
---
# <a name="get-educationschool"></a><span data-ttu-id="f2349-103">EducationSchool abrufen</span><span class="sxs-lookup"><span data-stu-id="f2349-103">Get educationSchool</span></span>

<span data-ttu-id="f2349-104">Abrufen der Eigenschaften und Beziehungen des Schulobjekts.</span><span class="sxs-lookup"><span data-stu-id="f2349-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2349-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2349-105">Permissions</span></span>
<span data-ttu-id="f2349-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2349-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2349-108">Permission type</span></span>      | <span data-ttu-id="f2349-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2349-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2349-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2349-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f2349-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="f2349-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="f2349-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2349-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f2349-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2349-113">Not supported.</span></span>  |
|<span data-ttu-id="f2349-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2349-114">Application</span></span> | <span data-ttu-id="f2349-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2349-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f2349-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2349-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2349-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f2349-117">Optional query parameters</span></span>
<span data-ttu-id="f2349-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2349-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2349-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2349-119">Request headers</span></span>
| <span data-ttu-id="f2349-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2349-120">Header</span></span>       | <span data-ttu-id="f2349-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f2349-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2349-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2349-122">Authorization</span></span>  | <span data-ttu-id="f2349-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2349-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2349-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2349-125">Request body</span></span>
<span data-ttu-id="f2349-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f2349-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f2349-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2349-127">Response</span></span>
<span data-ttu-id="f2349-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2349-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2349-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2349-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2349-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2349-130">Request</span></span>
<span data-ttu-id="f2349-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2349-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="f2349-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2349-132">Response</span></span>
<span data-ttu-id="f2349-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2349-133">The following is an example of the response.</span></span> 

><span data-ttu-id="f2349-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f2349-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
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