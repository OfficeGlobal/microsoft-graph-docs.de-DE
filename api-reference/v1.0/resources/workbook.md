# <a name="workbook-resource-type"></a><span data-ttu-id="032e4-101">Ressourcentyp „workbook“</span><span class="sxs-lookup"><span data-stu-id="032e4-101">Workbook resource type</span></span>

<span data-ttu-id="032e4-102">Die Arbeitsmappe ist das Objekt auf oberster Ebene, das dazugehörige Arbeitsmappenobjekte wie z. B. Arbeitsblätter, Tabellen, Bereiche usw. enthält.</span><span class="sxs-lookup"><span data-stu-id="032e4-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="json-representation"></a><span data-ttu-id="032e4-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="032e4-103">JSON representation</span></span>

<span data-ttu-id="032e4-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="032e4-104">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbook"
}-->

```json
{
  "names": [{"@odata.type": "microsoft.graph.workbookNamedItem"}],
  "tables": [{"@odata.type": "microsoft.graph.workbookTable"}],
  "worksheets": [{"@odata.type": "microsoft.graph.workbookWorksheet"}]
}
```

## <a name="properties"></a><span data-ttu-id="032e4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="032e4-105">Properties</span></span>
<span data-ttu-id="032e4-106">Keine</span><span class="sxs-lookup"><span data-stu-id="032e4-106">None</span></span>

## <a name="methods"></a><span data-ttu-id="032e4-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="032e4-107">Methods</span></span>

| <span data-ttu-id="032e4-108">Methode</span><span class="sxs-lookup"><span data-stu-id="032e4-108">Method</span></span>       | <span data-ttu-id="032e4-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="032e4-109">Return Type</span></span>  |<span data-ttu-id="032e4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="032e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="032e4-111">Sitzung erstellen</span><span class="sxs-lookup"><span data-stu-id="032e4-111">Create Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="032e4-112">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="032e4-112">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="032e4-113">Erstellen Sie eine Arbeitsmappensitzung, um eine dauerhafte oder nicht-beständige Sitzung zu starten.</span><span class="sxs-lookup"><span data-stu-id="032e4-113">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="032e4-114">Sitzung schließen</span><span class="sxs-lookup"><span data-stu-id="032e4-114">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="032e4-115">Keine</span><span class="sxs-lookup"><span data-stu-id="032e4-115">None</span></span> |<span data-ttu-id="032e4-116">Schließen Sie eine vorhandene Sitzung.</span><span class="sxs-lookup"><span data-stu-id="032e4-116">Close an existing session.</span></span>|
|[<span data-ttu-id="032e4-117">Sitzung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="032e4-117">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="032e4-118">Keine</span><span class="sxs-lookup"><span data-stu-id="032e4-118">None</span></span> |<span data-ttu-id="032e4-119">Aktualisieren Sie eine vorhandene Sitzung.</span><span class="sxs-lookup"><span data-stu-id="032e4-119">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="032e4-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="032e4-120">Relationships</span></span>
| <span data-ttu-id="032e4-121">Beziehung</span><span class="sxs-lookup"><span data-stu-id="032e4-121">Relationship</span></span> | <span data-ttu-id="032e4-122">Typ</span><span class="sxs-lookup"><span data-stu-id="032e4-122">Type</span></span>   |<span data-ttu-id="032e4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="032e4-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="032e4-124">names</span><span class="sxs-lookup"><span data-stu-id="032e4-124">names</span></span>|<span data-ttu-id="032e4-125">[WorkbookNamedItem](nameditem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="032e4-125">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="032e4-p101">Stellt eine Auflistung der benannten Elemente des Arbeitsmappenbereichs dar (benannte Bereiche und Konstanten). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="032e4-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="032e4-128">Tabellen</span><span class="sxs-lookup"><span data-stu-id="032e4-128">tables</span></span>|<span data-ttu-id="032e4-129">[WorkbookTable](table.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="032e4-129">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="032e4-p102">Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Tabellen dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="032e4-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="032e4-132">worksheets</span><span class="sxs-lookup"><span data-stu-id="032e4-132">worksheets</span></span>|<span data-ttu-id="032e4-133">[WorkbookWorksheet](worksheet.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="032e4-133">[WorkbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="032e4-p103">Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Arbeitsblätter dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="032e4-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="032e4-136">Funktionen</span><span class="sxs-lookup"><span data-stu-id="032e4-136">Functions</span></span>

<span data-ttu-id="032e4-p104">[Excel-Funktionen](#functions): Sie können eine Arbeitsmappenfunktion mit der Syntax `POST /workbook/functions/{function-name}` aufrufen. Geben Sie dabei die Funktionsargumente in Form eines JSON-Objekts im Text an. Der berechnete `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben. Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="032e4-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="032e4-p105">Eine vollständige Liste der unterstützten Funktionen finden Sie [hier](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Die Namen der einzelnen Parameter sowie die Datentypen finden Sie in der Funktionssignatur.</span><span class="sxs-lookup"><span data-stu-id="032e4-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="032e4-142">_Wichtige Hinweise:_</span><span class="sxs-lookup"><span data-stu-id="032e4-142">_Important notes:_</span></span> 
* <span data-ttu-id="032e4-143">Der Eingabebereichsparameter wird über ein Bereichsobjekt definiert, nicht über eine Bereichsadresszeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="032e4-143">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="032e4-144">Der Indexparameter startet die Indexierung bei 1; die in den meisten anderen APIs genutzte Indexierung ab 0 wird nicht verwendet.</span><span class="sxs-lookup"><span data-stu-id="032e4-144">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="032e4-145">Beispiel: **SVERWEIS**</span><span class="sxs-lookup"><span data-stu-id="032e4-145">Example: **vlookup**</span></span>

<span data-ttu-id="032e4-146">In einer Excel-Tabelle verwendet die `vlookup`-Funktion die folgenden Argumente an:</span><span class="sxs-lookup"><span data-stu-id="032e4-146">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="032e4-147">Der Wert, den Sie nachschlagen möchten, auch das Nachschlagewert bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="032e4-147">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="032e4-148">Der Bereich, in dem sich der Nachschlagewert befindet.</span><span class="sxs-lookup"><span data-stu-id="032e4-148">The range where the lookup value is located.</span></span> <span data-ttu-id="032e4-149">Denken Sie daran, dass sich der Nachschlagewert immer in der ersten Spalte des Bereichs für SVERWEIS befinden muss, um ordnungsgemäß zu funktionieren.</span><span class="sxs-lookup"><span data-stu-id="032e4-149">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="032e4-150">Wenn sich der Nachschlagewert beispielsweise in Zelle C2 befindet, sollte der Bereich mit C beginnen.</span><span class="sxs-lookup"><span data-stu-id="032e4-150">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="032e4-151">Die Spaltennummer im Bereich, die den Rückgabewert enthält.</span><span class="sxs-lookup"><span data-stu-id="032e4-151">The column number in the range that contains the return value.</span></span> <span data-ttu-id="032e4-152">Wenn Sie z. B. B2: D11 als Bereich angeben, sollten Sie B als erste Spalte, C als zweite Spalte usw. zählen.</span><span class="sxs-lookup"><span data-stu-id="032e4-152">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="032e4-153">Optional können Sie TRUE angeben, wenn Sie eine ungefähre Übereinstimmung wünschen, oder FALSE, wenn Sie eine genaue Übereinstimmung des Rückgabewerts möchten.</span><span class="sxs-lookup"><span data-stu-id="032e4-153">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="032e4-154">Wenn Sie nichts angeben, ist der Standardwert immer TRUE oder eine ungefähre Übereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="032e4-154">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="032e4-155">Innerhalb einer Zelle sieht die `vlookup`-Funktion folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="032e4-155">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="032e4-156">= SVERWEIS (Nachschlagewert, Bereich mit dem Nachschlagewert, Spaltennummer im Bereich mit dem Rückgabewert, geben Sie optional TRUE für eine ungefähre Übereinstimmung oder FALSE für eine genaue Übereinstimmung an)</span><span class="sxs-lookup"><span data-stu-id="032e4-156">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="032e4-157">(Sehen Sie sich die Dokumentation für die [SVERWEIS-Excel-Funktion](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1) an.)</span><span class="sxs-lookup"><span data-stu-id="032e4-157">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="032e4-158">Im folgenden Beispiel sehen Sie, wie Sie die `vlookup`-Funktion aufrufen und diese Parameter mit der Excel-REST-API weitergeben.</span><span class="sxs-lookup"><span data-stu-id="032e4-158">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="032e4-159">Anforderung:</span><span class="sxs-lookup"><span data-stu-id="032e4-159">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

<span data-ttu-id="032e4-160">Antwort:</span><span class="sxs-lookup"><span data-stu-id="032e4-160">Response:</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="032e4-161">Beispiel: `median`</span><span class="sxs-lookup"><span data-stu-id="032e4-161">Example: `median`</span></span>

<span data-ttu-id="032e4-162">In einer Excel-Tabelle verwendet die `median`-Funktion ein Array eines oder mehrerer Eingabebereiche.</span><span class="sxs-lookup"><span data-stu-id="032e4-162">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="032e4-163">Innerhalb einer Zelle sieht die `median`-Funktion folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="032e4-163">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="032e4-164">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="032e4-164">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="032e4-165">(Sehen Sie sich die Dokumentation für die [MEDIAN-Excel-Funktion](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2) an.)</span><span class="sxs-lookup"><span data-stu-id="032e4-165">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="032e4-166">Im folgenden Beispiel sehen Sie, wie Sie die `median`-Funktion und einen oder mehrere Eingabebereiche mit der Excel-REST-API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="032e4-166">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="032e4-167">Anforderung:</span><span class="sxs-lookup"><span data-stu-id="032e4-167">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ] 
}
```

<span data-ttu-id="032e4-168">Antwort:</span><span class="sxs-lookup"><span data-stu-id="032e4-168">Response:</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
