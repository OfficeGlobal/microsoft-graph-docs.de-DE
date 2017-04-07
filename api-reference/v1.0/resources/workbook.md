# <a name="workbook-resource-type"></a>Ressourcentyp „workbook“

Die Arbeitsmappe ist das Objekt auf oberster Ebene , das dazugehörige Arbeitsmappenobjekte wie z. B. Arbeitsblätter, Tabellen, Bereiche usw. enthält.

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|names|[NamedItem](nameditem.md) collection|Stellt eine Auflistung der benannten Elemente des Arbeitsmappenbereichs dar (benannte Bereiche und Konstanten). Schreibgeschützt.|
|Tabellen|[Table](table.md) collection|Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Tabellen dar. Schreibgeschützt.|
|worksheets|[Worksheet](worksheet.md) collection|Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Arbeitsblätter dar. Schreibgeschützt.|

## <a name="functions"></a>Funktionen

[Excel-Funktionen](#functions): Sie können eine Arbeitsmappenfunktion mit der Syntax `POST /workbook/functions/{function-name}` aufrufen. Geben Sie dabei die Funktionsargumente in Form eines JSON-Objekts im Text an. Der berechnete `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben. Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde. 

Eine vollständige Liste der unterstützten Funktionen finden Sie [hier](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Die Namen der einzelnen Parameter sowie die Datentypen finden Sie in der Funktionssignatur.

_Wichtige Hinweise:_ 
* Der Eingabebereichsparameter wird über ein Bereichsobjekt definiert, nicht über eine Bereichsadresszeichenfolge.  
* Der Indexparameter startet die Indexierung bei 1; die in den meisten anderen APIs genutzte Indexierung ab 0 wird nicht verwendet. 

Beispiel: 

Im Beispiel unten wird die Funktion `vlookup` aufgerufen, indem der Suchwert, der Eingabebereich und der zurückzugebende Wert übergeben werden. 

Anforderung: 

```http 
POST https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
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

Antwort:

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

Beispiel: 

Im Beispiel unten wird die Funktion `median` aufgerufen, indem die Eingabebereiche in einem Array übergeben werden. 

Anforderung: 

```http 
POST https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/median
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

Antwort:

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
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
