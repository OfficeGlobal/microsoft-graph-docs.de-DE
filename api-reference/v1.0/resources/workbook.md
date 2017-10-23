# <a name="workbook-resource-type"></a><span data-ttu-id="bb6f9-101">Ressourcentyp „workbook“</span><span class="sxs-lookup"><span data-stu-id="bb6f9-101">Workbook resource type</span></span>

<span data-ttu-id="bb6f9-102">Die Arbeitsmappe ist das Objekt auf oberster Ebene , das dazugehörige Arbeitsmappenobjekte wie z. B. Arbeitsblätter, Tabellen, Bereiche usw. enthält.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="bb6f9-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb6f9-103">Properties</span></span>
<span data-ttu-id="bb6f9-104">Keine</span><span class="sxs-lookup"><span data-stu-id="bb6f9-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="bb6f9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb6f9-105">Methods</span></span>

| <span data-ttu-id="bb6f9-106">Methode</span><span class="sxs-lookup"><span data-stu-id="bb6f9-106">Method</span></span>       | <span data-ttu-id="bb6f9-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bb6f9-107">Return Type</span></span>  |<span data-ttu-id="bb6f9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb6f9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb6f9-109">Create Session</span><span class="sxs-lookup"><span data-stu-id="bb6f9-109">Create Upload Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="bb6f9-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="bb6f9-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="bb6f9-111">Erstellen Sie eine Arbeitsmappensitzung, um eine dauerhafte oder nicht-beständige Sitzung zu starten.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="bb6f9-112">Close Session</span><span class="sxs-lookup"><span data-stu-id="bb6f9-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="bb6f9-113">Keine</span><span class="sxs-lookup"><span data-stu-id="bb6f9-113">None</span></span> |<span data-ttu-id="bb6f9-114">Schließen Sie eine vorhandene Sitzung.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-114">Close an existing session.</span></span>|
|[<span data-ttu-id="bb6f9-115">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="bb6f9-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="bb6f9-116">Keine</span><span class="sxs-lookup"><span data-stu-id="bb6f9-116">None</span></span> |<span data-ttu-id="bb6f9-117">Aktualisieren Sie eine vorhandene Sitzung.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="bb6f9-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb6f9-118">Relationships</span></span>
| <span data-ttu-id="bb6f9-119">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bb6f9-119">Relationship</span></span> | <span data-ttu-id="bb6f9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="bb6f9-120">Type</span></span>   |<span data-ttu-id="bb6f9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb6f9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb6f9-122">names</span><span class="sxs-lookup"><span data-stu-id="bb6f9-122">names</span></span>|<span data-ttu-id="bb6f9-123">[NamedItem](nameditem.md) collection</span><span class="sxs-lookup"><span data-stu-id="bb6f9-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="bb6f9-p101">Stellt eine Auflistung der benannten Elemente des Arbeitsmappenbereichs dar (benannte Bereiche und Konstanten). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="bb6f9-126">tables</span><span class="sxs-lookup"><span data-stu-id="bb6f9-126">tables</span></span>|<span data-ttu-id="bb6f9-127">[Table](table.md) collection</span><span class="sxs-lookup"><span data-stu-id="bb6f9-127">[Table](table.md) collection</span></span>|<span data-ttu-id="bb6f9-p102">Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Tabellen dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="bb6f9-130">worksheets</span><span class="sxs-lookup"><span data-stu-id="bb6f9-130">worksheets</span></span>|<span data-ttu-id="bb6f9-131">[Worksheet](worksheet.md) collection</span><span class="sxs-lookup"><span data-stu-id="bb6f9-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="bb6f9-p103">Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Arbeitsblätter dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="bb6f9-134">Funktionen</span><span class="sxs-lookup"><span data-stu-id="bb6f9-134">Functions</span></span>

<span data-ttu-id="bb6f9-135">[Excel-Funktionen](#functions): Sie können eine Arbeitsmappenfunktion mit der Syntax `POST /workbook/functions/{function-name}` aufrufen. Geben Sie dabei die Funktionsargumente in Form eines JSON-Objekts im Text an.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting  and any  strings are returned in the function result object. The  value of  indicates successful execution of the function.</span></span> <span data-ttu-id="bb6f9-136">Der berechnete `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="bb6f9-137">Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="bb6f9-138">Eine vollständige Liste der unterstützten Funktionen finden Sie [hier](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="bb6f9-138">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span> <span data-ttu-id="bb6f9-139">Die Namen der einzelnen Parameter sowie die Datentypen finden Sie in der Funktionssignatur.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-139">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="bb6f9-140">_Wichtige Hinweise:_</span><span class="sxs-lookup"><span data-stu-id="bb6f9-140">_Important notes:_</span></span> 
* <span data-ttu-id="bb6f9-141">Der Eingabebereichsparameter wird über ein Bereichsobjekt definiert, nicht über eine Bereichsadresszeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="bb6f9-142">Der Indexparameter startet die Indexierung bei 1; die in den meisten anderen APIs genutzte Indexierung ab 0 wird nicht verwendet.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="bb6f9-143">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="bb6f9-143">Example:</span></span> 

<span data-ttu-id="bb6f9-144">Im Beispiel unten wird die Funktion `vlookup` aufgerufen, indem der Suchwert, der Eingabebereich und der zurückzugebende Wert übergeben werden.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-144">In the below example, `vlookup` function is called by passing lookup value, input range and the value to be returned.</span></span> 

<span data-ttu-id="bb6f9-145">Anforderung:</span><span class="sxs-lookup"><span data-stu-id="bb6f9-145">Request:</span></span> 

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

<span data-ttu-id="bb6f9-146">Antwort:</span><span class="sxs-lookup"><span data-stu-id="bb6f9-146">Response:</span></span>

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="bb6f9-147">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="bb6f9-147">Example:</span></span> 

<span data-ttu-id="bb6f9-148">Im Beispiel unten wird die Funktion `median` aufgerufen, indem die Eingabebereiche in einem Array übergeben werden.</span><span class="sxs-lookup"><span data-stu-id="bb6f9-148">In the below example, `median` function is called by passing the input range(s) in an array.</span></span> 

<span data-ttu-id="bb6f9-149">Anforderung:</span><span class="sxs-lookup"><span data-stu-id="bb6f9-149">Request:</span></span> 

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

<span data-ttu-id="bb6f9-150">Antwort:</span><span class="sxs-lookup"><span data-stu-id="bb6f9-150">Response:</span></span>

```http
HTTP code: 200, OK
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
