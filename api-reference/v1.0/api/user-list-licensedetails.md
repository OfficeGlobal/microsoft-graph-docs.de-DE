---
title: licenseDetails auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 7f9869088e7ee6e8f4857ad3f8a7c4e3768e529b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826523"
---
# <a name="list-licensedetails"></a><span data-ttu-id="f0d28-103">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="f0d28-103">List licenseDetails</span></span>

<span data-ttu-id="f0d28-104">Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="f0d28-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0d28-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0d28-105">Permissions</span></span>
<span data-ttu-id="f0d28-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0d28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0d28-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0d28-108">Permission type</span></span>      | <span data-ttu-id="f0d28-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f0d28-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0d28-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0d28-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0d28-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0d28-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f0d28-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0d28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0d28-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="f0d28-113">User.Read</span></span>    |
|<span data-ttu-id="f0d28-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0d28-114">Application</span></span> | <span data-ttu-id="f0d28-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0d28-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0d28-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0d28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0d28-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f0d28-117">Optional query parameters</span></span>
<span data-ttu-id="f0d28-118">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="f0d28-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0d28-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0d28-119">Request headers</span></span>
| <span data-ttu-id="f0d28-120">Name</span><span class="sxs-lookup"><span data-stu-id="f0d28-120">Name</span></span>      |<span data-ttu-id="f0d28-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0d28-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0d28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d28-122">Authorization</span></span>  | <span data-ttu-id="f0d28-123">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="f0d28-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0d28-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0d28-124">Request body</span></span>
<span data-ttu-id="f0d28-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f0d28-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0d28-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0d28-126">Response</span></span>

<span data-ttu-id="f0d28-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [licenseDetails](../resources/licensedetails.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0d28-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0d28-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0d28-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0d28-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0d28-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="f0d28-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0d28-130">Response</span></span>
<span data-ttu-id="f0d28-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0d28-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
