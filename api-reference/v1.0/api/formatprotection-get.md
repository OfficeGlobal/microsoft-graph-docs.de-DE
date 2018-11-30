---
title: FormatProtection abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des formatProtection-Objekts.
ms.openlocfilehash: 4c586d070b506dd0ab10db8291863e051137f840
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017956"
---
# <a name="get-formatprotection"></a><span data-ttu-id="ea2e8-103">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="ea2e8-103">Get FormatProtection</span></span>

<span data-ttu-id="ea2e8-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-104">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea2e8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ea2e8-105">Permissions</span></span>
<span data-ttu-id="ea2e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea2e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea2e8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea2e8-108">Permission type</span></span>      | <span data-ttu-id="ea2e8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea2e8-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ea2e8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea2e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea2e8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea2e8-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="ea2e8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea2e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea2e8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea2e8-113">Not supported.</span></span>    | 
|<span data-ttu-id="ea2e8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea2e8-114">Application</span></span> | <span data-ttu-id="ea2e8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea2e8-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ea2e8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea2e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea2e8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ea2e8-117">Optional query parameters</span></span>
<span data-ttu-id="ea2e8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea2e8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea2e8-119">Request headers</span></span>
| <span data-ttu-id="ea2e8-120">Name</span><span class="sxs-lookup"><span data-stu-id="ea2e8-120">Name</span></span>      |<span data-ttu-id="ea2e8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea2e8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea2e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea2e8-122">Authorization</span></span>  | <span data-ttu-id="ea2e8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ea2e8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea2e8-125">Request body</span></span>
<span data-ttu-id="ea2e8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea2e8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea2e8-127">Response</span></span>

<span data-ttu-id="ea2e8-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-128">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea2e8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea2e8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea2e8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea2e8-130">Request</span></span>
<span data-ttu-id="ea2e8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="ea2e8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea2e8-132">Response</span></span>
<span data-ttu-id="ea2e8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea2e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->