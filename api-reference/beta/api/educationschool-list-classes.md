---
title: EducationClasses auflisten
description: Abrufen einer Liste von Klassen im Besitz einer Schule.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4d4dacca2530b183639222aba6d7d306b64b07dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883566"
---
# <a name="list-educationclasses"></a><span data-ttu-id="99e51-103">EducationClasses auflisten</span><span class="sxs-lookup"><span data-stu-id="99e51-103">List educationClasses</span></span>

> <span data-ttu-id="99e51-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99e51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99e51-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99e51-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99e51-106">Abrufen einer Liste von Klassen im Besitz einer Schule.</span><span class="sxs-lookup"><span data-stu-id="99e51-106">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="99e51-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99e51-107">Permissions</span></span>
<span data-ttu-id="99e51-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e51-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99e51-110">Permission type</span></span>      | <span data-ttu-id="99e51-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99e51-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e51-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99e51-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="99e51-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="99e51-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="99e51-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99e51-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="99e51-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99e51-115">Not supported.</span></span>  |
|<span data-ttu-id="99e51-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99e51-116">Application</span></span> | <span data-ttu-id="99e51-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e51-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="99e51-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99e51-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99e51-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="99e51-119">Optional query parameters</span></span>
<span data-ttu-id="99e51-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="99e51-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99e51-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99e51-121">Request headers</span></span>
| <span data-ttu-id="99e51-122">Header</span><span class="sxs-lookup"><span data-stu-id="99e51-122">Header</span></span>       | <span data-ttu-id="99e51-123">Wert</span><span class="sxs-lookup"><span data-stu-id="99e51-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99e51-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e51-124">Authorization</span></span>  | <span data-ttu-id="99e51-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99e51-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99e51-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99e51-127">Request body</span></span>
<span data-ttu-id="99e51-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="99e51-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="99e51-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="99e51-129">Response</span></span>
<span data-ttu-id="99e51-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99e51-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99e51-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99e51-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99e51-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99e51-132">Request</span></span>
<span data-ttu-id="99e51-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99e51-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
##### <a name="response"></a><span data-ttu-id="99e51-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="99e51-134">Response</span></span>
<span data-ttu-id="99e51-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="99e51-135">The following is an example of the response.</span></span> 

><span data-ttu-id="99e51-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="99e51-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
