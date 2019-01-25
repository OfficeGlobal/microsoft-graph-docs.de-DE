---
title: 'TableColumnCollection: add'
description: Fügt der Tabelle eine neue Spalte hinzu.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1f3e2b5cacb3bb7ab462cc127b9cbc2e3b85019f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529110"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="cf38a-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="cf38a-103">TableColumnCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf38a-104">Fügt der Tabelle eine neue Spalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="cf38a-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf38a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf38a-105">Permissions</span></span>
<span data-ttu-id="cf38a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf38a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf38a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf38a-108">Permission type</span></span>      | <span data-ttu-id="cf38a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf38a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf38a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf38a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf38a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf38a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf38a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf38a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf38a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf38a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf38a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf38a-114">Application</span></span> | <span data-ttu-id="cf38a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf38a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf38a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf38a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="cf38a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf38a-117">Request headers</span></span>
| <span data-ttu-id="cf38a-118">Name</span><span class="sxs-lookup"><span data-stu-id="cf38a-118">Name</span></span>       | <span data-ttu-id="cf38a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf38a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf38a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf38a-120">Authorization</span></span>  | <span data-ttu-id="cf38a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf38a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf38a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cf38a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cf38a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cf38a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf38a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf38a-126">Request body</span></span>
<span data-ttu-id="cf38a-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cf38a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf38a-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="cf38a-128">Parameter</span></span>    | <span data-ttu-id="cf38a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cf38a-129">Type</span></span>   |<span data-ttu-id="cf38a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf38a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf38a-131">Index</span><span class="sxs-lookup"><span data-stu-id="cf38a-131">index</span></span>|<span data-ttu-id="cf38a-132">number</span><span class="sxs-lookup"><span data-stu-id="cf38a-132">number</span></span>|<span data-ttu-id="cf38a-p104">Gibt die relative Position der neuen Spalte an. Die vorherige Spalte an dieser Position wird nach rechts verschoben. Der Indexwert sollte gleich oder kleiner als der letzten Spalten-Indexwert sein, damit er nicht dazu verwendet werden kann, eine Spalte an das Ende der Tabelle anzuhängen. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="cf38a-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="cf38a-137">values</span><span class="sxs-lookup"><span data-stu-id="cf38a-137">values</span></span>|<span data-ttu-id="cf38a-138">(boolean or string or number)</span><span class="sxs-lookup"><span data-stu-id="cf38a-138">(boolean or string or number)</span></span>|<span data-ttu-id="cf38a-p105">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenspalte.</span><span class="sxs-lookup"><span data-stu-id="cf38a-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="cf38a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf38a-141">Response</span></span>

<span data-ttu-id="cf38a-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf38a-142">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf38a-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf38a-143">Example</span></span>
<span data-ttu-id="cf38a-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="cf38a-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf38a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf38a-145">Request</span></span>
<span data-ttu-id="cf38a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf38a-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="cf38a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf38a-147">Response</span></span>
<span data-ttu-id="cf38a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf38a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
