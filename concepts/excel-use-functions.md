# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a><span data-ttu-id="a48be-101">Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a48be-101">Use workbook functions in Excel with Microsoft Graph</span></span>

<span data-ttu-id="a48be-102">Mithilfe der Syntax `POST /workbook/functions/{function-name}` können Sie jede beliebige Arbeitsmappenfunktion aufrufen.</span><span class="sxs-lookup"><span data-stu-id="a48be-102">You can invoke any workbook function by using the following syntax: `POST /workbook/functions/{function-name}`.</span></span> <span data-ttu-id="a48be-103">Die Funktionsargumente werden in Form eines JSON-Objekts im Text angegeben.</span><span class="sxs-lookup"><span data-stu-id="a48be-103">You provide the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="a48be-104">Der Ergebniswert `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a48be-104">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="a48be-105">Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="a48be-105">The `error` value of `null` indicates successful execution of the function.</span></span>

<span data-ttu-id="a48be-106">Eine vollständige Liste der unterstützten Funktionen finden Sie [hier](https://support.office.com/de-DE/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="a48be-106">The complete list of supported functions are listed [here](https://support.office.com/de-DE/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span></span> <span data-ttu-id="a48be-107">Die Namen der einzelnen Parameter sowie die Datentypen finden Sie in der Funktionssignatur.</span><span class="sxs-lookup"><span data-stu-id="a48be-107">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="a48be-108">_Wichtige Hinweise:_</span><span class="sxs-lookup"><span data-stu-id="a48be-108">_Important notes:_</span></span>
* <span data-ttu-id="a48be-109">Der Eingabebereichsparameter wird über ein Bereichsobjekt definiert, nicht über eine Bereichsadresszeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="a48be-109">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="a48be-110">Der Indexparameter startet die Indexierung bei 1; die in den meisten anderen APIs genutzte Indexierung ab 0 wird nicht verwendet.</span><span class="sxs-lookup"><span data-stu-id="a48be-110">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span>

<span data-ttu-id="a48be-111">Beispiel: **SVERWEIS**</span><span class="sxs-lookup"><span data-stu-id="a48be-111">Example: **vlookup**</span></span>

<span data-ttu-id="a48be-112">In einer Excel-Tabelle können mit der Funktion `vlookup` folgende Argumente verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="a48be-112">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="a48be-113">**lookup_value** (erforderlich): Der Wert, der nachgeschlagen werden soll.</span><span class="sxs-lookup"><span data-stu-id="a48be-113">**lookup_value** (required) The value you want to look up.</span></span>
2. <span data-ttu-id="a48be-114">**table_array** (erforderlich): Der Zellenbereich, in dem sich der Nachschlagewert befindet.</span><span class="sxs-lookup"><span data-stu-id="a48be-114">**table_array** (required) The range of cells where the lookup value is located.</span></span> <span data-ttu-id="a48be-115">Denken Sie daran, dass sich der Nachschlagewert immer in der ersten Spalte des Bereichs befinden muss, damit „vlookup“ korrekt funktioniert.</span><span class="sxs-lookup"><span data-stu-id="a48be-115">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="a48be-116">Wenn sich der Nachschlagewert beispielsweise in Zelle C2 befindet, muss der Bereich mit C beginnen.</span><span class="sxs-lookup"><span data-stu-id="a48be-116">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="a48be-117">**col_index_num** (erforderlich): Die Spaltennummer in dem Bereich, der den Rückgabewert enthält.</span><span class="sxs-lookup"><span data-stu-id="a48be-117">The column number in the range that contains the return value.</span></span> <span data-ttu-id="a48be-118">Wenn Sie z. B. B2: D11 als Bereich angeben, sollten Sie B als erste Spalte, C als zweite Spalte usw. zählen.</span><span class="sxs-lookup"><span data-stu-id="a48be-118">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="a48be-119">**range_lookup** (optional): Der logische Wert, der angibt, ob **vlookup** nach einer ungefähren Übereinstimmung oder einer exakten Übereinstimmung suchen soll.</span><span class="sxs-lookup"><span data-stu-id="a48be-119">**range_lookup** (optional) The logical value that specifies whether you want **VLOOKUP** to find an approximate or an exact match.</span></span> <span data-ttu-id="a48be-120">Setzen Sie den Wert auf **TRUE**, wenn eine ungefähre Übereinstimmung mit dem Rückgabewert gesucht werden soll, und auf **FALSE**, wenn eine exakte Übereinstimmung gesucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="a48be-120">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="a48be-121">Wenn Sie keinen Wert angeben, wird als Standardwert immer „TRUE“ gesetzt, d. h. es wird nach einer ungefähren Übereinstimmung gesucht.</span><span class="sxs-lookup"><span data-stu-id="a48be-121">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="a48be-122">Innerhalb einer Zelle sieht die `vlookup`-Funktion folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="a48be-122">Inside a cell, the `vlookup` function looks like this:</span></span>

<span data-ttu-id="a48be-123">= SVERWEIS (Nachschlagewert, Bereich mit dem Nachschlagewert, Spaltennummer im Bereich mit dem Rückgabewert, geben Sie optional TRUE für eine ungefähre Übereinstimmung oder FALSE für eine genaue Übereinstimmung an)</span><span class="sxs-lookup"><span data-stu-id="a48be-123">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="a48be-124">(Details finden Sie in der Dokumentation zur [Excel-Funktion „vlookup“](https://support.office.com/de-DE/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span><span class="sxs-lookup"><span data-stu-id="a48be-124">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/de-DE/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>


##### <a name="request"></a><span data-ttu-id="a48be-125">Anforderung:</span><span class="sxs-lookup"><span data-stu-id="a48be-125">Request:</span></span>
<span data-ttu-id="a48be-126">Das folgende Beispiel illustriert, wie Sie mit der Excel-REST-API die Funktion `vlookup` aufrufen und diese Parameter übergeben können.</span><span class="sxs-lookup"><span data-stu-id="a48be-126">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a48be-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a48be-127">Response</span></span>

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

<span data-ttu-id="a48be-128">Beispiel: `median`</span><span class="sxs-lookup"><span data-stu-id="a48be-128">Example: `median`</span></span>

<span data-ttu-id="a48be-129">In einer Excel-Tabelle verwendet die `median`-Funktion ein Array eines oder mehrerer Eingabebereiche.</span><span class="sxs-lookup"><span data-stu-id="a48be-129">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="a48be-130">Innerhalb einer Zelle sieht die `median`-Funktion folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="a48be-130">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="a48be-131">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="a48be-131">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="a48be-132">(Details finden Sie in der Dokumentation zur [Excel-Funktion „MEDIAN“](https://support.office.com/de-DE/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span><span class="sxs-lookup"><span data-stu-id="a48be-132">(See the documentation for the [MEDIAN Excel function](https://support.office.com/de-DE/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

##### <a name="request"></a><span data-ttu-id="a48be-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a48be-133">Request</span></span>
<span data-ttu-id="a48be-134">Im folgenden Beispiel sehen Sie, wie Sie mit der Excel-REST-API die Funktion `median` sowie einen oder mehrere Eingabebereiche aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="a48be-134">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a48be-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a48be-135">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a48be-136">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="a48be-136">See also</span></span>
* [<span data-ttu-id="a48be-137">Verwalten von Sitzungen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a48be-137">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="a48be-138">Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a48be-138">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="a48be-139">Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a48be-139">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="a48be-140">Display a chart image in Excel with Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a48be-140">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="a48be-141">Verwenden der Excel-REST-API</span><span class="sxs-lookup"><span data-stu-id="a48be-141">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)
