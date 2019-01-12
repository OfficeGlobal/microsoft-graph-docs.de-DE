---
title: EducationClasses auflisten
description: Abrufen einer Liste von Klassen im Besitz einer Schule.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d49e8094e28cf8c5901bfd36d9e9af02c97e2eee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991510"
---
# <a name="list-educationclasses"></a><span data-ttu-id="67c64-103">EducationClasses auflisten</span><span class="sxs-lookup"><span data-stu-id="67c64-103">List educationClasses</span></span>

<span data-ttu-id="67c64-104">Abrufen einer Liste von Klassen im Besitz einer Schule.</span><span class="sxs-lookup"><span data-stu-id="67c64-104">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="67c64-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67c64-105">Permissions</span></span>
<span data-ttu-id="67c64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67c64-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67c64-108">Permission type</span></span>      | <span data-ttu-id="67c64-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67c64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67c64-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67c64-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67c64-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="67c64-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="67c64-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67c64-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="67c64-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67c64-113">Not supported.</span></span>  |
|<span data-ttu-id="67c64-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67c64-114">Application</span></span> | <span data-ttu-id="67c64-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c64-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="67c64-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67c64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67c64-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="67c64-117">Optional query parameters</span></span>
<span data-ttu-id="67c64-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="67c64-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67c64-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67c64-119">Request headers</span></span>
| <span data-ttu-id="67c64-120">Header</span><span class="sxs-lookup"><span data-stu-id="67c64-120">Header</span></span>       | <span data-ttu-id="67c64-121">Wert</span><span class="sxs-lookup"><span data-stu-id="67c64-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67c64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c64-122">Authorization</span></span>  | <span data-ttu-id="67c64-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67c64-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67c64-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67c64-125">Request body</span></span>
<span data-ttu-id="67c64-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="67c64-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67c64-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="67c64-127">Response</span></span>
<span data-ttu-id="67c64-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67c64-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67c64-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67c64-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67c64-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67c64-130">Request</span></span>
<span data-ttu-id="67c64-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67c64-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
##### <a name="response"></a><span data-ttu-id="67c64-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="67c64-132">Response</span></span>
<span data-ttu-id="67c64-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="67c64-133">The following is an example of the response.</span></span> 

><span data-ttu-id="67c64-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="67c64-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
