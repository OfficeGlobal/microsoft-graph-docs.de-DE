---
title: TableColumn erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 17c49101decad6ad840ff8c564e204ccd6399072
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981224"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="57905-103">TableColumn erstellen</span><span class="sxs-lookup"><span data-stu-id="57905-103">Create TableColumn</span></span>

<span data-ttu-id="57905-104">Verwenden Sie diese API zum Erstellen einer neuen TableColumn.</span><span class="sxs-lookup"><span data-stu-id="57905-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="57905-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="57905-105">Permissions</span></span>
<span data-ttu-id="57905-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57905-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57905-108">Permission type</span></span>      | <span data-ttu-id="57905-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57905-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57905-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57905-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57905-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57905-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57905-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57905-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57905-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57905-113">Not supported.</span></span>    |
|<span data-ttu-id="57905-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57905-114">Application</span></span> | <span data-ttu-id="57905-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57905-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57905-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57905-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="57905-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57905-117">Request headers</span></span>
| <span data-ttu-id="57905-118">Name</span><span class="sxs-lookup"><span data-stu-id="57905-118">Name</span></span>       | <span data-ttu-id="57905-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57905-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57905-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="57905-120">Authorization</span></span>  | <span data-ttu-id="57905-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="57905-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57905-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="57905-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="57905-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="57905-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57905-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57905-126">Request body</span></span>
<span data-ttu-id="57905-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [WorkbookTableColumn](../resources/tablecolumn.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="57905-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57905-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="57905-128">Response</span></span>

<span data-ttu-id="57905-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und [WorkbookTableColumn](../resources/tablecolumn.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="57905-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57905-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57905-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57905-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57905-131">Request</span></span>
<span data-ttu-id="57905-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57905-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="57905-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [WorkbookTableColumn](../resources/tablecolumn.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="57905-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="57905-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="57905-134">Response</span></span>
<span data-ttu-id="57905-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57905-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
