---
title: Ressourcentyp „workbook“
description: Die Arbeitsmappe ist das Objekt auf oberster Ebene , das dazugehörige Arbeitsmappenobjekte wie z. B. Arbeitsblätter, Tabellen, Bereiche usw. enthält.
ms.openlocfilehash: 6575cc2d49e4b30e78e07989f38600ae64d5c5a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018048"
---
# <a name="workbook-resource-type"></a>Ressourcentyp „workbook“

Die Arbeitsmappe ist das Objekt auf oberster Ebene , das dazugehörige Arbeitsmappenobjekte wie z. B. Arbeitsblätter, Tabellen, Bereiche usw. enthält.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

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

## <a name="properties"></a>Eigenschaften
Keine

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Create Session](../api/workbook-createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |Erstellen Sie eine Arbeitsmappensitzung, um eine dauerhafte oder nicht-beständige Sitzung zu starten.|
|[Close Session](../api/workbook-closesession.md) | Keine |Schließen Sie eine vorhandene Sitzung.|
|[Refresh Session](../api/workbook-refreshsession.md) | Keine |Aktualisieren Sie eine vorhandene Sitzung.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|names|[WorkbookNamedItem](nameditem.md) -Auflistung|Stellt eine Auflistung der benannten Elemente des Arbeitsmappenbereichs dar (benannte Bereiche und Konstanten). Schreibgeschützt.|
|Tabellen|[WorkbookTable](table.md) -Auflistung|Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Tabellen dar. Schreibgeschützt.|
|worksheets|[WorkbookWorksheet](worksheet.md) -Auflistung|Stellt eine Auflistung der mit der Arbeitsmappe verknüpften Arbeitsblätter dar. Schreibgeschützt.|

## <a name="functions"></a>Funktionen

[Excel-Funktionen](#functions): Sie können eine Arbeitsmappenfunktion mit der Syntax `POST /workbook/functions/{function-name}` aufrufen. Geben Sie dabei die Funktionsargumente in Form eines JSON-Objekts im Text an. Der berechnete `value` der Funktion sowie alle Zeichenfolgen des Typs `error` werden im Funktionsergebnisobjekt zurückgegeben. Wird für den Wert `error` `null` zurückgegeben, bedeutet das, dass die Funktion erfolgreich ausgeführt wurde. 

Eine vollständige Liste der unterstützten Funktionen finden Sie [hier](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Die Namen der einzelnen Parameter sowie die Datentypen finden Sie in der Funktionssignatur.

_Wichtige Hinweise:_ 
* Der Eingabebereichsparameter wird über ein Bereichsobjekt definiert, nicht über eine Bereichsadresszeichenfolge.  
* Der Indexparameter startet die Indexierung bei 1; die in den meisten anderen APIs genutzte Indexierung ab 0 wird nicht verwendet. 

Beispiel: **SVERWEIS**

In einer Excel-Tabelle verwendet die `vlookup`-Funktion die folgenden Argumente an:

1. Der Wert, den Sie nachschlagen möchten, auch das Nachschlagewert bezeichnet.
2. Der Bereich, in dem sich der Nachschlagewert befindet. Denken Sie daran, dass sich der Nachschlagewert immer in der ersten Spalte des Bereichs für SVERWEIS befinden muss, um ordnungsgemäß zu funktionieren. Wenn sich der Nachschlagewert beispielsweise in Zelle C2 befindet, sollte der Bereich mit C beginnen.
3. Die Spaltennummer im Bereich, die den Rückgabewert enthält. Wenn Sie z. B. B2: D11 als Bereich angeben, sollten Sie B als erste Spalte, C als zweite Spalte usw. zählen.
4. Optional können Sie TRUE angeben, wenn Sie eine ungefähre Übereinstimmung wünschen, oder FALSE, wenn Sie eine genaue Übereinstimmung des Rückgabewerts möchten. Wenn Sie nichts angeben, ist der Standardwert immer TRUE oder eine ungefähre Übereinstimmung.

Innerhalb einer Zelle sieht die `vlookup`-Funktion folgendermaßen aus: 

= SVERWEIS (Nachschlagewert, Bereich mit dem Nachschlagewert, Spaltennummer im Bereich mit dem Rückgabewert, geben Sie optional TRUE für eine ungefähre Übereinstimmung oder FALSE für eine genaue Übereinstimmung an)

(Sehen Sie sich die Dokumentation für die [SVERWEIS-Excel-Funktion](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1) an.)

Im folgenden Beispiel sehen Sie, wie Sie die `vlookup`-Funktion aufrufen und diese Parameter mit der Excel-REST-API weitergeben.

Anforderung: 

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

Antwort:

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

(Sehen Sie sich die Dokumentation für die [MEDIAN-Excel-Funktion](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2) an.)

Im folgenden Beispiel sehen Sie, wie Sie die `median`-Funktion und einen oder mehrere Eingabebereiche mit der Excel-REST-API aufrufen. 

Anforderung: 

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

Antwort:

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
