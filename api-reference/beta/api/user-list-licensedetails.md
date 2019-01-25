---
title: licenseDetails auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7dae02120f17dfbd329758734ba5fb912adfe0e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515944"
---
# <a name="list-licensedetails"></a><span data-ttu-id="1acbc-103">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="1acbc-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1acbc-104">Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="1acbc-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1acbc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1acbc-105">Permissions</span></span>
<span data-ttu-id="1acbc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1acbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1acbc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1acbc-108">Permission type</span></span>      | <span data-ttu-id="1acbc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1acbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1acbc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1acbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1acbc-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1acbc-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1acbc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1acbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1acbc-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="1acbc-113">User.Read</span></span>    |
|<span data-ttu-id="1acbc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1acbc-114">Application</span></span> | <span data-ttu-id="1acbc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1acbc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1acbc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1acbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1acbc-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1acbc-117">Optional query parameters</span></span>
<span data-ttu-id="1acbc-118">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="1acbc-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1acbc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1acbc-119">Request headers</span></span>
| <span data-ttu-id="1acbc-120">Name</span><span class="sxs-lookup"><span data-stu-id="1acbc-120">Name</span></span>      |<span data-ttu-id="1acbc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1acbc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1acbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1acbc-122">Authorization</span></span>  | <span data-ttu-id="1acbc-123">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="1acbc-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="1acbc-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1acbc-124">Request body</span></span>
<span data-ttu-id="1acbc-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1acbc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1acbc-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="1acbc-126">Response</span></span>

<span data-ttu-id="1acbc-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [licenseDetails](../resources/licensedetails.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1acbc-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1acbc-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1acbc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1acbc-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1acbc-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="1acbc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1acbc-130">Response</span></span>
<span data-ttu-id="1acbc-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1acbc-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
