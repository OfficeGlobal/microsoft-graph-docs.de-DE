---
title: TableRow erstellen
description: 'Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. '
ms.openlocfilehash: c7a4340005f7eaea60d95c806475de92373e1364
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060367"
---
# <a name="create-tablerow"></a><span data-ttu-id="e943e-108">TableRow erstellen</span><span class="sxs-lookup"><span data-stu-id="e943e-108">Create TableRow</span></span>

> <span data-ttu-id="e943e-109">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e943e-109">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e943e-110">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e943e-110">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e943e-111">Fügt Zeilen an das Ende der Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="e943e-111">Adds rows to the end of the table.</span></span> <span data-ttu-id="e943e-112">Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann.</span><span class="sxs-lookup"><span data-stu-id="e943e-112">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="e943e-113">Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen.</span><span class="sxs-lookup"><span data-stu-id="e943e-113">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="e943e-114">Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen.</span><span class="sxs-lookup"><span data-stu-id="e943e-114">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="e943e-115">Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="e943e-115">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="e943e-116">Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="e943e-116">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="e943e-117">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="e943e-117">Error Handling</span></span>

<span data-ttu-id="e943e-118">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="e943e-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="e943e-119">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e943e-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="e943e-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e943e-120">Permissions</span></span>
<span data-ttu-id="e943e-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e943e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e943e-123">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e943e-123">Permission type</span></span>      | <span data-ttu-id="e943e-124">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e943e-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e943e-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e943e-125">Delegated (work or school account)</span></span> | <span data-ttu-id="e943e-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e943e-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e943e-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e943e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e943e-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e943e-128">Not supported.</span></span>    |
|<span data-ttu-id="e943e-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e943e-129">Application</span></span> | <span data-ttu-id="e943e-130">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e943e-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e943e-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e943e-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="e943e-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e943e-132">Request headers</span></span>
| <span data-ttu-id="e943e-133">Name</span><span class="sxs-lookup"><span data-stu-id="e943e-133">Name</span></span>       | <span data-ttu-id="e943e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e943e-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e943e-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="e943e-135">Authorization</span></span>  | <span data-ttu-id="e943e-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e943e-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e943e-138">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e943e-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="e943e-p107">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e943e-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e943e-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e943e-141">Request body</span></span>
<span data-ttu-id="e943e-142">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e943e-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e943e-143">Parameter</span><span class="sxs-lookup"><span data-stu-id="e943e-143">Parameter</span></span>    | <span data-ttu-id="e943e-144">Typ</span><span class="sxs-lookup"><span data-stu-id="e943e-144">Type</span></span>   |<span data-ttu-id="e943e-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e943e-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e943e-146">Index</span><span class="sxs-lookup"><span data-stu-id="e943e-146">index</span></span>|<span data-ttu-id="e943e-147">number</span><span class="sxs-lookup"><span data-stu-id="e943e-147">number</span></span>|<span data-ttu-id="e943e-p108">Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="e943e-p108">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="e943e-153">values</span><span class="sxs-lookup"><span data-stu-id="e943e-153">values</span></span>|<span data-ttu-id="e943e-154">(boolean or string or number)</span><span class="sxs-lookup"><span data-stu-id="e943e-154">(boolean or string or number)</span></span>|<span data-ttu-id="e943e-155">Ein 2-dimensionales Array der unformatierte Werte der Tabellenzeilen.</span><span class="sxs-lookup"><span data-stu-id="e943e-155">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="e943e-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="e943e-156">Response</span></span>

<span data-ttu-id="e943e-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e943e-157">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e943e-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e943e-158">Example</span></span>
<span data-ttu-id="e943e-159">In diesem Beispiel werden zwei Zeilen mit Daten an das Ende der Tabelle eingefügt.</span><span class="sxs-lookup"><span data-stu-id="e943e-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="e943e-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e943e-160">Request</span></span>
<span data-ttu-id="e943e-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e943e-161">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="e943e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="e943e-162">Response</span></span>
<span data-ttu-id="e943e-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e943e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->
