---
title: licenseDetails auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.
author: dkershaw10
ms.openlocfilehash: af15e2cf8fb2bb9484d4567517c71a735f11609c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301071"
---
# <a name="list-licensedetails"></a><span data-ttu-id="b9189-103">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="b9189-103">List licenseDetails</span></span>

<span data-ttu-id="b9189-104">Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="b9189-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9189-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9189-105">Permissions</span></span>
<span data-ttu-id="b9189-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9189-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9189-108">Permission type</span></span>      | <span data-ttu-id="b9189-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9189-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9189-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9189-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9189-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9189-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9189-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9189-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9189-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="b9189-113">User.Read</span></span>    |
|<span data-ttu-id="b9189-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9189-114">Application</span></span> | <span data-ttu-id="b9189-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9189-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9189-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9189-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9189-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b9189-117">Optional query parameters</span></span>
<span data-ttu-id="b9189-118">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="b9189-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9189-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9189-119">Request headers</span></span>
| <span data-ttu-id="b9189-120">Name</span><span class="sxs-lookup"><span data-stu-id="b9189-120">Name</span></span>      |<span data-ttu-id="b9189-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9189-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9189-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9189-122">Authorization</span></span>  | <span data-ttu-id="b9189-123">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="b9189-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9189-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9189-124">Request body</span></span>
<span data-ttu-id="b9189-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9189-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9189-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9189-126">Response</span></span>

<span data-ttu-id="b9189-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [licenseDetails](../resources/licensedetails.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9189-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9189-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9189-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9189-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9189-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="b9189-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9189-130">Response</span></span>
<span data-ttu-id="b9189-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9189-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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