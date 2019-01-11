---
title: licenseDetails auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f000cc390673887a7708f8615769416cbc2204b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863357"
---
# <a name="list-licensedetails"></a><span data-ttu-id="00a7a-103">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="00a7a-103">List licenseDetails</span></span>

> <span data-ttu-id="00a7a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00a7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00a7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00a7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00a7a-106">Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="00a7a-106">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="00a7a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="00a7a-107">Permissions</span></span>
<span data-ttu-id="00a7a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a7a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00a7a-110">Permission type</span></span>      | <span data-ttu-id="00a7a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00a7a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00a7a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00a7a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00a7a-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00a7a-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00a7a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00a7a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00a7a-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="00a7a-115">User.Read</span></span>    |
|<span data-ttu-id="00a7a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00a7a-116">Application</span></span> | <span data-ttu-id="00a7a-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a7a-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00a7a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00a7a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="00a7a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="00a7a-119">Optional query parameters</span></span>
<span data-ttu-id="00a7a-120">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="00a7a-120">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="00a7a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00a7a-121">Request headers</span></span>
| <span data-ttu-id="00a7a-122">Name</span><span class="sxs-lookup"><span data-stu-id="00a7a-122">Name</span></span>      |<span data-ttu-id="00a7a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00a7a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00a7a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="00a7a-124">Authorization</span></span>  | <span data-ttu-id="00a7a-125">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="00a7a-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a7a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00a7a-126">Request body</span></span>
<span data-ttu-id="00a7a-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="00a7a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00a7a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="00a7a-128">Response</span></span>

<span data-ttu-id="00a7a-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [licenseDetails](../resources/licensedetails.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00a7a-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00a7a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00a7a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00a7a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00a7a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="00a7a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="00a7a-132">Response</span></span>
<span data-ttu-id="00a7a-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00a7a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
