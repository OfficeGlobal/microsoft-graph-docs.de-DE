---
title: EducationClasses auflisten
description: Abrufen einer Liste von Klassen im Besitz einer Schule.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47f15ecb7678e9d3a18c42324deb87e0e2c8dffd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516791"
---
# <a name="list-educationclasses"></a><span data-ttu-id="ef18a-103">EducationClasses auflisten</span><span class="sxs-lookup"><span data-stu-id="ef18a-103">List educationClasses</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef18a-104">Abrufen einer Liste von Klassen im Besitz einer Schule.</span><span class="sxs-lookup"><span data-stu-id="ef18a-104">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef18a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef18a-105">Permissions</span></span>
<span data-ttu-id="ef18a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef18a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef18a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef18a-108">Permission type</span></span>      | <span data-ttu-id="ef18a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef18a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef18a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef18a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ef18a-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ef18a-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="ef18a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef18a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ef18a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef18a-113">Not supported.</span></span>  |
|<span data-ttu-id="ef18a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef18a-114">Application</span></span> | <span data-ttu-id="ef18a-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef18a-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ef18a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef18a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef18a-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ef18a-117">Optional query parameters</span></span>
<span data-ttu-id="ef18a-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef18a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef18a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef18a-119">Request headers</span></span>
| <span data-ttu-id="ef18a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef18a-120">Header</span></span>       | <span data-ttu-id="ef18a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ef18a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef18a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef18a-122">Authorization</span></span>  | <span data-ttu-id="ef18a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef18a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef18a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef18a-125">Request body</span></span>
<span data-ttu-id="ef18a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef18a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ef18a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef18a-127">Response</span></span>
<span data-ttu-id="ef18a-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef18a-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef18a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef18a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef18a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef18a-130">Request</span></span>
<span data-ttu-id="ef18a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef18a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
##### <a name="response"></a><span data-ttu-id="ef18a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef18a-132">Response</span></span>
<span data-ttu-id="ef18a-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef18a-133">The following is an example of the response.</span></span> 

><span data-ttu-id="ef18a-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ef18a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-list-classes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
