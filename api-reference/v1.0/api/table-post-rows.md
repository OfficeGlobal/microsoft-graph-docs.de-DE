---
title: TableRow erstellen
description: 'Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. '
localization_priority: Normal
ms.openlocfilehash: 27979ee3f6ed38d9815e78a29b17f07bb72bcf91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840138"
---
# <a name="create-tablerow"></a><span data-ttu-id="1d307-108">TableRow erstellen</span><span class="sxs-lookup"><span data-stu-id="1d307-108">Create TableRow</span></span>

<span data-ttu-id="1d307-109">Fügt Zeilen an das Ende der Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="1d307-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="1d307-110">Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann.</span><span class="sxs-lookup"><span data-stu-id="1d307-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="1d307-111">Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen.</span><span class="sxs-lookup"><span data-stu-id="1d307-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="1d307-112">Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen.</span><span class="sxs-lookup"><span data-stu-id="1d307-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="1d307-113">Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="1d307-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="1d307-114">Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="1d307-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="1d307-115">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="1d307-115">Error Handling</span></span>

<span data-ttu-id="1d307-116">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="1d307-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="1d307-117">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d307-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d307-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1d307-118">Permissions</span></span>
<span data-ttu-id="1d307-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d307-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d307-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d307-121">Permission type</span></span>      | <span data-ttu-id="1d307-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d307-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d307-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d307-123">Delegated (work or school account)</span></span> | <span data-ttu-id="1d307-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d307-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d307-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d307-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d307-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d307-126">Not supported.</span></span>    |
|<span data-ttu-id="1d307-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d307-127">Application</span></span> | <span data-ttu-id="1d307-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d307-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d307-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d307-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="1d307-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d307-130">Request headers</span></span>
| <span data-ttu-id="1d307-131">Name</span><span class="sxs-lookup"><span data-stu-id="1d307-131">Name</span></span>       | <span data-ttu-id="1d307-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d307-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d307-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d307-133">Authorization</span></span>  | <span data-ttu-id="1d307-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d307-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d307-136">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1d307-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="1d307-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1d307-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d307-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d307-139">Request body</span></span>
<span data-ttu-id="1d307-140">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1d307-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d307-141">Parameter</span><span class="sxs-lookup"><span data-stu-id="1d307-141">Parameter</span></span>    | <span data-ttu-id="1d307-142">Typ</span><span class="sxs-lookup"><span data-stu-id="1d307-142">Type</span></span>   |<span data-ttu-id="1d307-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d307-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d307-144">Index</span><span class="sxs-lookup"><span data-stu-id="1d307-144">index</span></span>|<span data-ttu-id="1d307-145">number</span><span class="sxs-lookup"><span data-stu-id="1d307-145">number</span></span>|<span data-ttu-id="1d307-p107">Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="1d307-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="1d307-151">values</span><span class="sxs-lookup"><span data-stu-id="1d307-151">values</span></span>|<span data-ttu-id="1d307-152">Json</span><span class="sxs-lookup"><span data-stu-id="1d307-152">Json</span></span>|<span data-ttu-id="1d307-153">Ein 2-dimensionales Array der unformatierte Werte der Tabellenzeilen (Boolean oder Zeichenfolge oder Zahl).</span><span class="sxs-lookup"><span data-stu-id="1d307-153">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="1d307-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d307-154">Response</span></span>

<span data-ttu-id="1d307-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d307-155">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d307-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d307-156">Example</span></span>
<span data-ttu-id="1d307-157">In diesem Beispiel werden zwei Zeilen mit Daten an das Ende der Tabelle eingefügt.</span><span class="sxs-lookup"><span data-stu-id="1d307-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="1d307-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d307-158">Request</span></span>
<span data-ttu-id="1d307-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d307-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
##### <a name="response"></a><span data-ttu-id="1d307-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d307-160">Response</span></span>
<span data-ttu-id="1d307-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d307-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/v1.0/api/table-post-rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table-post-rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->
