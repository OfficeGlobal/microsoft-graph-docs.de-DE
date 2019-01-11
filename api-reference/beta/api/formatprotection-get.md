---
title: FormatProtection abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des formatProtection-Objekts.
localization_priority: Normal
ms.openlocfilehash: c8588e6fc33c1fe5b1bf761a6408b1e3d2f77b8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883699"
---
# <a name="get-formatprotection"></a><span data-ttu-id="55b63-103">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="55b63-103">Get FormatProtection</span></span>

> <span data-ttu-id="55b63-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="55b63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55b63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55b63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55b63-106">Dient zum Abrufen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="55b63-106">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55b63-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="55b63-107">Permissions</span></span>
<span data-ttu-id="55b63-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55b63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b63-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55b63-110">Permission type</span></span>      | <span data-ttu-id="55b63-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55b63-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55b63-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55b63-112">Delegated (work or school account)</span></span> | <span data-ttu-id="55b63-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55b63-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55b63-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55b63-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55b63-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55b63-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55b63-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55b63-116">Application</span></span> | <span data-ttu-id="55b63-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55b63-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55b63-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55b63-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55b63-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="55b63-119">Optional query parameters</span></span>
<span data-ttu-id="55b63-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55b63-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55b63-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55b63-121">Request headers</span></span>
| <span data-ttu-id="55b63-122">Name</span><span class="sxs-lookup"><span data-stu-id="55b63-122">Name</span></span>      |<span data-ttu-id="55b63-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55b63-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55b63-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="55b63-124">Authorization</span></span>  | <span data-ttu-id="55b63-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55b63-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55b63-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55b63-127">Request body</span></span>
<span data-ttu-id="55b63-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55b63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55b63-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="55b63-129">Response</span></span>

<span data-ttu-id="55b63-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55b63-130">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55b63-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55b63-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55b63-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55b63-132">Request</span></span>
<span data-ttu-id="55b63-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55b63-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="55b63-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="55b63-134">Response</span></span>
<span data-ttu-id="55b63-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55b63-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
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
