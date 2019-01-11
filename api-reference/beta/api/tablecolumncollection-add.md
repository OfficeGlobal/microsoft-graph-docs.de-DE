---
title: 'TableColumnCollection: add'
description: Fügt der Tabelle eine neue Spalte hinzu.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: bd3c1a2b1cbfcb8d0e47f9d7ec93b0695e9854c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870238"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="dc533-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="dc533-103">TableColumnCollection: add</span></span>

> <span data-ttu-id="dc533-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dc533-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc533-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dc533-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc533-106">Fügt der Tabelle eine neue Spalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="dc533-106">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc533-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dc533-107">Permissions</span></span>
<span data-ttu-id="dc533-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc533-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc533-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc533-110">Permission type</span></span>      | <span data-ttu-id="dc533-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc533-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc533-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc533-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc533-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc533-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc533-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc533-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc533-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc533-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc533-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc533-116">Application</span></span> | <span data-ttu-id="dc533-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc533-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc533-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc533-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="dc533-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc533-119">Request headers</span></span>
| <span data-ttu-id="dc533-120">Name</span><span class="sxs-lookup"><span data-stu-id="dc533-120">Name</span></span>       | <span data-ttu-id="dc533-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc533-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc533-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc533-122">Authorization</span></span>  | <span data-ttu-id="dc533-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc533-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc533-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="dc533-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc533-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="dc533-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc533-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc533-128">Request body</span></span>
<span data-ttu-id="dc533-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="dc533-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc533-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="dc533-130">Parameter</span></span>    | <span data-ttu-id="dc533-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dc533-131">Type</span></span>   |<span data-ttu-id="dc533-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc533-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc533-133">Index</span><span class="sxs-lookup"><span data-stu-id="dc533-133">index</span></span>|<span data-ttu-id="dc533-134">number</span><span class="sxs-lookup"><span data-stu-id="dc533-134">number</span></span>|<span data-ttu-id="dc533-p105">Gibt die relative Position der neuen Spalte an. Die vorherige Spalte an dieser Position wird nach rechts verschoben. Der Indexwert sollte gleich oder kleiner als der letzten Spalten-Indexwert sein, damit er nicht dazu verwendet werden kann, eine Spalte an das Ende der Tabelle anzuhängen. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="dc533-p105">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="dc533-139">values</span><span class="sxs-lookup"><span data-stu-id="dc533-139">values</span></span>|<span data-ttu-id="dc533-140">(boolean or string or number)</span><span class="sxs-lookup"><span data-stu-id="dc533-140">(boolean or string or number)</span></span>|<span data-ttu-id="dc533-p106">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenspalte.</span><span class="sxs-lookup"><span data-stu-id="dc533-p106">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="dc533-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc533-143">Response</span></span>

<span data-ttu-id="dc533-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc533-144">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc533-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc533-145">Example</span></span>
<span data-ttu-id="dc533-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="dc533-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc533-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc533-147">Request</span></span>
<span data-ttu-id="dc533-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc533-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dc533-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc533-149">Response</span></span>
<span data-ttu-id="dc533-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc533-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
