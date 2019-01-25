---
title: Klassen auflisten
description: 'Abrufen einer Liste von Klassenobjekten. Hinweis: Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Klassen. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: c7af59ec2198609ef1efaf12b87b89f0d251df01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515076"
---
# <a name="list-classes"></a><span data-ttu-id="3a001-104">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="3a001-104">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a001-105">Abrufen einer Liste von Klassenobjekten.</span><span class="sxs-lookup"><span data-stu-id="3a001-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="3a001-106">Hinweis: Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Klassen.</span><span class="sxs-lookup"><span data-stu-id="3a001-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="3a001-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a001-107">Permissions</span></span>
<span data-ttu-id="3a001-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a001-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a001-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a001-110">Permission type</span></span>      | <span data-ttu-id="3a001-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a001-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a001-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a001-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a001-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3a001-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3a001-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a001-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3a001-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a001-115">Not supported.</span></span>  |
|<span data-ttu-id="3a001-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a001-116">Application</span></span> | <span data-ttu-id="3a001-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a001-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a001-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a001-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a001-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3a001-119">Optional query parameters</span></span>
<span data-ttu-id="3a001-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a001-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a001-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a001-121">Request headers</span></span>
| <span data-ttu-id="3a001-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3a001-122">Header</span></span>       | <span data-ttu-id="3a001-123">Wert</span><span class="sxs-lookup"><span data-stu-id="3a001-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a001-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a001-124">Authorization</span></span>  | <span data-ttu-id="3a001-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a001-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a001-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a001-127">Request body</span></span>
<span data-ttu-id="3a001-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a001-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3a001-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a001-129">Response</span></span>
<span data-ttu-id="3a001-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a001-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a001-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a001-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a001-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a001-132">Request</span></span>
<span data-ttu-id="3a001-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a001-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="3a001-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a001-134">Response</span></span>
<span data-ttu-id="3a001-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a001-135">The following is an example of the response.</span></span> 

><span data-ttu-id="3a001-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3a001-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/educationuser-list-classes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
