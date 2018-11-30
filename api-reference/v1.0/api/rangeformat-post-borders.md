---
title: RangeBorder erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen RangeBorder.
ms.openlocfilehash: 22a0e85a0e4e2ca6ad0a4fb2bdf503a01c892452
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016884"
---
# <a name="create-rangeborder"></a><span data-ttu-id="98963-103">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="98963-103">Create RangeBorder</span></span>

<span data-ttu-id="98963-104">Verwenden Sie diese API zum Erstellen eines neuen RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="98963-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="98963-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98963-105">Permissions</span></span>
<span data-ttu-id="98963-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98963-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98963-108">Permission type</span></span>      | <span data-ttu-id="98963-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98963-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98963-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98963-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98963-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98963-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98963-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98963-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98963-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98963-113">Not supported.</span></span>    |
|<span data-ttu-id="98963-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98963-114">Application</span></span> | <span data-ttu-id="98963-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98963-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98963-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98963-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="98963-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98963-117">Request headers</span></span>
| <span data-ttu-id="98963-118">Name</span><span class="sxs-lookup"><span data-stu-id="98963-118">Name</span></span>       | <span data-ttu-id="98963-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98963-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98963-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98963-120">Authorization</span></span>  | <span data-ttu-id="98963-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="98963-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98963-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="98963-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="98963-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="98963-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98963-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98963-126">Request body</span></span>
<span data-ttu-id="98963-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [WorkbookRangeBorder](../resources/rangeborder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="98963-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98963-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="98963-128">Response</span></span>

<span data-ttu-id="98963-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und [WorkbookRangeBorder](../resources/rangeborder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="98963-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98963-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98963-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98963-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98963-131">Request</span></span>
<span data-ttu-id="98963-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="98963-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="98963-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [WorkbookRangeBorder](../resources/rangeborder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="98963-133">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="98963-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="98963-134">Response</span></span>
<span data-ttu-id="98963-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98963-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->