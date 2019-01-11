---
title: Klassen auflisten
description: 'Abrufen einer Liste von Klassenobjekten. Hinweis: Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Klassen. '
localization_priority: Normal
ms.openlocfilehash: f5cde95f6dc577a0f0330d2ead9291c07db47053
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809198"
---
# <a name="list-classes"></a><span data-ttu-id="95f0e-104">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="95f0e-104">List classes</span></span>

> <span data-ttu-id="95f0e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="95f0e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95f0e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="95f0e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95f0e-107">Abrufen einer Liste von Klassenobjekten.</span><span class="sxs-lookup"><span data-stu-id="95f0e-107">Retrieve a list of class objects.</span></span> <span data-ttu-id="95f0e-108">Hinweis: Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Klassen.</span><span class="sxs-lookup"><span data-stu-id="95f0e-108">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="95f0e-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="95f0e-109">Permissions</span></span>
<span data-ttu-id="95f0e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95f0e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95f0e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="95f0e-112">Permission type</span></span>      | <span data-ttu-id="95f0e-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="95f0e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95f0e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="95f0e-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="95f0e-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="95f0e-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="95f0e-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="95f0e-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="95f0e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95f0e-117">Not supported.</span></span>  |
|<span data-ttu-id="95f0e-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="95f0e-118">Application</span></span> | <span data-ttu-id="95f0e-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f0e-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="95f0e-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="95f0e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95f0e-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="95f0e-121">Optional query parameters</span></span>
<span data-ttu-id="95f0e-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="95f0e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95f0e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="95f0e-123">Request headers</span></span>
| <span data-ttu-id="95f0e-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="95f0e-124">Header</span></span>       | <span data-ttu-id="95f0e-125">Wert</span><span class="sxs-lookup"><span data-stu-id="95f0e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95f0e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="95f0e-126">Authorization</span></span>  | <span data-ttu-id="95f0e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="95f0e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95f0e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="95f0e-129">Request body</span></span>
<span data-ttu-id="95f0e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="95f0e-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="95f0e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="95f0e-131">Response</span></span>
<span data-ttu-id="95f0e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="95f0e-132">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95f0e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="95f0e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95f0e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="95f0e-134">Request</span></span>
<span data-ttu-id="95f0e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="95f0e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="95f0e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="95f0e-136">Response</span></span>
<span data-ttu-id="95f0e-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="95f0e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="95f0e-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="95f0e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
