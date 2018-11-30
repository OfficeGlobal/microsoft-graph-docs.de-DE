---
title: TableRow erstellen
description: 'Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. '
ms.openlocfilehash: 67197eb8ba67bfc4f8406de5df2d7158409c85d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019721"
---
# <a name="create-tablerow"></a>TableRow erstellen

Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. 

## <a name="error-handling"></a>Fehlerbehandlung

Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf. Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Arbeitsmappensitzungs-ID  | Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Index|number|Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.|
|values|Json|Ein 2-dimensionales Array der unformatierte Werte der Tabellenzeilen (Boolean oder Zeichenfolge oder Zahl).|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
In diesem Beispiel werden zwei Zeilen mit Daten an das Ende der Tabelle eingefügt. 

##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
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
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
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
