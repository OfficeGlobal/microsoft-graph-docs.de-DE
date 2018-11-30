---
title: 'TableRowCollection: add'
description: 'Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. '
ms.openlocfilehash: fc2b89a25ade4b9d85844716370d95d52689de9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017537"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="0bf2d-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="0bf2d-108">TableRowCollection: add</span></span>

<span data-ttu-id="0bf2d-109">Fügt Zeilen an das Ende der Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="0bf2d-110">Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="0bf2d-111">Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="0bf2d-112">Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="0bf2d-113">Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="0bf2d-114">Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="0bf2d-115">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="0bf2d-115">Error Handling</span></span>

<span data-ttu-id="0bf2d-116">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="0bf2d-117">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bf2d-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0bf2d-118">Permissions</span></span>
<span data-ttu-id="0bf2d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bf2d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bf2d-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bf2d-121">Permission type</span></span>      | <span data-ttu-id="0bf2d-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bf2d-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bf2d-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bf2d-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0bf2d-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bf2d-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0bf2d-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bf2d-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bf2d-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bf2d-126">Not supported.</span></span>    |
|<span data-ttu-id="0bf2d-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bf2d-127">Application</span></span> | <span data-ttu-id="0bf2d-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bf2d-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bf2d-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bf2d-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="0bf2d-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bf2d-130">Request headers</span></span>
| <span data-ttu-id="0bf2d-131">Name</span><span class="sxs-lookup"><span data-stu-id="0bf2d-131">Name</span></span>       | <span data-ttu-id="0bf2d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bf2d-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0bf2d-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bf2d-133">Authorization</span></span>  | <span data-ttu-id="0bf2d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bf2d-136">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0bf2d-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="0bf2d-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bf2d-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bf2d-139">Request body</span></span>
<span data-ttu-id="0bf2d-140">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0bf2d-141">Parameter</span><span class="sxs-lookup"><span data-stu-id="0bf2d-141">Parameter</span></span>    | <span data-ttu-id="0bf2d-142">Typ</span><span class="sxs-lookup"><span data-stu-id="0bf2d-142">Type</span></span>   |<span data-ttu-id="0bf2d-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bf2d-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bf2d-144">Index</span><span class="sxs-lookup"><span data-stu-id="0bf2d-144">index</span></span>|<span data-ttu-id="0bf2d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0bf2d-145">Int32</span></span>|<span data-ttu-id="0bf2d-p107">Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="0bf2d-151">values</span><span class="sxs-lookup"><span data-stu-id="0bf2d-151">values</span></span>|<span data-ttu-id="0bf2d-152">Json</span><span class="sxs-lookup"><span data-stu-id="0bf2d-152">Json</span></span>|<span data-ttu-id="0bf2d-p108">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenzeile.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-p108">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="0bf2d-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bf2d-155">Response</span></span>

<span data-ttu-id="0bf2d-156">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookTableRow](../resources/tablerow.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-156">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bf2d-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bf2d-157">Example</span></span>
<span data-ttu-id="0bf2d-158">In diesem Beispiel werden zwei Zeilen mit Daten an das Ende der Tabelle eingefügt.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-158">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="0bf2d-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bf2d-159">Request</span></span>
<span data-ttu-id="0bf2d-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="0bf2d-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bf2d-161">Response</span></span>
<span data-ttu-id="0bf2d-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bf2d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
