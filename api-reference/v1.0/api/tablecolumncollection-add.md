---
title: 'TableColumnCollection: add'
description: Fügt der Tabelle eine neue Spalte hinzu.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b736f5bb6bcfac78701fbfd0aae75c0d84e34416
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840145"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="844f8-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="844f8-103">TableColumnCollection: add</span></span>

<span data-ttu-id="844f8-104">Fügt der Tabelle eine neue Spalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="844f8-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="844f8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="844f8-105">Permissions</span></span>
<span data-ttu-id="844f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="844f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="844f8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="844f8-108">Permission type</span></span>      | <span data-ttu-id="844f8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="844f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="844f8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="844f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="844f8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="844f8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="844f8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="844f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="844f8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="844f8-113">Not supported.</span></span>    |
|<span data-ttu-id="844f8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="844f8-114">Application</span></span> | <span data-ttu-id="844f8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="844f8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="844f8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="844f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="844f8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="844f8-117">Request headers</span></span>
| <span data-ttu-id="844f8-118">Name</span><span class="sxs-lookup"><span data-stu-id="844f8-118">Name</span></span>       | <span data-ttu-id="844f8-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="844f8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="844f8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="844f8-120">Authorization</span></span>  | <span data-ttu-id="844f8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="844f8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="844f8-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="844f8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="844f8-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="844f8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="844f8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="844f8-126">Request body</span></span>
<span data-ttu-id="844f8-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="844f8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="844f8-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="844f8-128">Parameter</span></span>    | <span data-ttu-id="844f8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="844f8-129">Type</span></span>   |<span data-ttu-id="844f8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="844f8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="844f8-131">Index</span><span class="sxs-lookup"><span data-stu-id="844f8-131">index</span></span>|<span data-ttu-id="844f8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="844f8-132">Int32</span></span>|<span data-ttu-id="844f8-p104">Gibt die relative Position der neuen Spalte an. Die vorherige Spalte an dieser Position wird nach rechts verschoben. Der Indexwert sollte gleich oder kleiner als der letzten Spalten-Indexwert sein, damit er nicht dazu verwendet werden kann, eine Spalte an das Ende der Tabelle anzuhängen. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="844f8-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="844f8-137">values</span><span class="sxs-lookup"><span data-stu-id="844f8-137">values</span></span>|<span data-ttu-id="844f8-138">Json</span><span class="sxs-lookup"><span data-stu-id="844f8-138">Json</span></span>|<span data-ttu-id="844f8-p105">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenspalte.</span><span class="sxs-lookup"><span data-stu-id="844f8-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="844f8-141">name</span><span class="sxs-lookup"><span data-stu-id="844f8-141">name</span></span>|<span data-ttu-id="844f8-142">string</span><span class="sxs-lookup"><span data-stu-id="844f8-142">string</span></span>|<span data-ttu-id="844f8-143">name</span><span class="sxs-lookup"><span data-stu-id="844f8-143">name</span></span>
## <a name="response"></a><span data-ttu-id="844f8-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="844f8-144">Response</span></span>

<span data-ttu-id="844f8-145">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookTableColumn](../resources/tablecolumn.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="844f8-145">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="844f8-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="844f8-146">Example</span></span>
<span data-ttu-id="844f8-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="844f8-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="844f8-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="844f8-148">Request</span></span>
<span data-ttu-id="844f8-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="844f8-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="844f8-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="844f8-150">Response</span></span>
<span data-ttu-id="844f8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="844f8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
