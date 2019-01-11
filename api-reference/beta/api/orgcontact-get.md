---
title: Abrufen von orgContact
description: Rufen Sie die Eigenschaften und Beziehungen des Orgcontact-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 4a806c48ef7fc9adc4a8eb94bc7c28e3add78d14
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842931"
---
# <a name="get-orgcontact"></a><span data-ttu-id="da10d-103">Abrufen von orgContact</span><span class="sxs-lookup"><span data-stu-id="da10d-103">Get orgContact</span></span>

> <span data-ttu-id="da10d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da10d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da10d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da10d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da10d-106">Rufen Sie die Eigenschaften und Beziehungen des Orgcontact-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="da10d-106">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da10d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="da10d-107">Permissions</span></span>
<span data-ttu-id="da10d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da10d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da10d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da10d-110">Permission type</span></span>      | <span data-ttu-id="da10d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da10d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da10d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da10d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da10d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da10d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da10d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da10d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da10d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da10d-115">Not supported.</span></span>    |
|<span data-ttu-id="da10d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da10d-116">Application</span></span> | <span data-ttu-id="da10d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da10d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da10d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da10d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da10d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="da10d-119">Optional query parameters</span></span>
<span data-ttu-id="da10d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="da10d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da10d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da10d-121">Request headers</span></span>
| <span data-ttu-id="da10d-122">Name</span><span class="sxs-lookup"><span data-stu-id="da10d-122">Name</span></span>       | <span data-ttu-id="da10d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="da10d-123">Type</span></span> | <span data-ttu-id="da10d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da10d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da10d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="da10d-125">Authorization</span></span>  | <span data-ttu-id="da10d-126">string</span><span class="sxs-lookup"><span data-stu-id="da10d-126">string</span></span>  | <span data-ttu-id="da10d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da10d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da10d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da10d-129">Request body</span></span>
<span data-ttu-id="da10d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da10d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da10d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="da10d-131">Response</span></span>

<span data-ttu-id="da10d-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OrgContact](../resources/orgcontact.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="da10d-132">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da10d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da10d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da10d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da10d-134">Request</span></span>
<span data-ttu-id="da10d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da10d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="da10d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="da10d-136">Response</span></span>
<span data-ttu-id="da10d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da10d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
