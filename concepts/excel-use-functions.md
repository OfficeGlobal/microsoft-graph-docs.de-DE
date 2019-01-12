---
title: Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph
description: Mithilfe der Syntax `POST /workbook/functions/{function-name}` können Sie jede beliebige Arbeitsmappenfunktion aufrufen. Die Funktionsargumente werden in Form eines JSON-Objekts im Text angegeben. Der Ergebniswert `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben. Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 868695eb6f3ab4ddd7354512477d4abcf0708d8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929977"
---
# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a>Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph

Mithilfe der Syntax `POST /workbook/functions/{function-name}` können Sie jede beliebige Arbeitsmappenfunktion aufrufen. Die Funktionsargumente werden in Form eines JSON-Objekts im Text angegeben. Der Ergebniswert `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben. Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde.

Eine vollständige Liste der unterstützten Funktionen finden Sie [hier](https://support.office.com/de-DE/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Die Namen der einzelnen Parameter sowie die Datentypen finden Sie in der Funktionssignatur.

_Wichtige Hinweise:_
* Der Eingabebereichsparameter wird über ein Bereichsobjekt definiert, nicht über eine Bereichsadresszeichenfolge.  
* Der Indexparameter startet die Indexierung bei 1; die in den meisten anderen APIs genutzte Indexierung ab 0 wird nicht verwendet.

Beispiel: **SVERWEIS**

In einer Excel-Tabelle können mit der Funktion `vlookup` folgende Argumente verwendet werden:

1. **lookup_value** (erforderlich): Der Wert, der nachgeschlagen werden soll.
2. **table_array** (erforderlich): Der Zellenbereich, in dem sich der Nachschlagewert befindet. Denken Sie daran, dass sich der Nachschlagewert immer in der ersten Spalte des Bereichs befinden muss, damit „vlookup“ korrekt funktioniert. Wenn sich der Nachschlagewert beispielsweise in Zelle C2 befindet, muss der Bereich mit C beginnen.
3. **col_index_num** (erforderlich): Die Spaltennummer in dem Bereich, der den Rückgabewert enthält. Wenn Sie z. B. B2: D11 als Bereich angeben, sollten Sie B als erste Spalte, C als zweite Spalte usw. zählen.
4. **range_lookup** (optional): Der logische Wert, der angibt, ob **vlookup** nach einer ungefähren Übereinstimmung oder einer exakten Übereinstimmung suchen soll. Setzen Sie den Wert auf **TRUE**, wenn eine ungefähre Übereinstimmung mit dem Rückgabewert gesucht werden soll, und auf **FALSE**, wenn eine exakte Übereinstimmung gesucht werden soll. Wenn Sie keinen Wert angeben, wird als Standardwert immer „TRUE“ gesetzt, d. h. es wird nach einer ungefähren Übereinstimmung gesucht.

Innerhalb einer Zelle sieht die `vlookup`-Funktion folgendermaßen aus:

= SVERWEIS (Nachschlagewert, Bereich mit dem Nachschlagewert, Spaltennummer im Bereich mit dem Rückgabewert, geben Sie optional TRUE für eine ungefähre Übereinstimmung oder FALSE für eine genaue Übereinstimmung an)

(Details finden Sie in der Dokumentation zur [Excel-Funktion „vlookup“](https://support.office.com/de-DE/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)


##### <a name="request"></a>Anforderung:
Das folgende Beispiel illustriert, wie Sie mit der Excel-REST-API die Funktion `vlookup` aufrufen und diese Parameter übergeben können.

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

##### <a name="response"></a>Antwort

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

Beispiel: `median`

In einer Excel-Tabelle verwendet die `median`-Funktion ein Array eines oder mehrerer Eingabebereiche.

Innerhalb einer Zelle sieht die `median`-Funktion folgendermaßen aus:

=MEDIAN(A2:A6)

(Details finden Sie in der Dokumentation zur [Excel-Funktion „MEDIAN“](https://support.office.com/de-DE/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)

##### <a name="request"></a>Anforderung
Im folgenden Beispiel sehen Sie, wie Sie mit der Excel-REST-API die Funktion `median` sowie einen oder mehrere Eingabebereiche aufrufen können.

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

##### <a name="response"></a>Antwort

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

## <a name="see-also"></a>Weitere Artikel
* [Verwalten von Sitzungen in Excel mit Microsoft Graph](excel-manage-sessions.md)
* [Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph](excel-write-to-workbook.md)
* [Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph](excel-update-range-format.md)
* [Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph](excel-display-chart-image.md)
* [Verwenden der Excel-REST-API](/graph/api/resources/excel?view=graph-rest-1.0)
