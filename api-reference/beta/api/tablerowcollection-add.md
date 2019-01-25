---
title: 'TableRowCollection: add'
description: 'Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fbc4d8d3b0f5a1653bf4d022dfea8c68c5401d18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523085"
---
# <a name="tablerowcollection-add"></a>TableRowCollection: add

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fügt Zeilen an das Ende der Tabelle an. Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann. Hinzufügen einer Zeile zu einem Zeitpunkt kann zu Leistungseinbußen führen. Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf anstatt einzelne Zeile einfügen. Um optimale Ergebnisse zu hinzufügen sammeln Zeilen, die auf der Anwendungsseite eingefügt werden, und führen Sie die einzelne Zeilen Vorgang. Probieren Sie die Anzahl der Zeilen, um die ideale Anzahl der Zeilen, die in den einzelnen API-Aufruf verwenden, zu bestimmen. 

## <a name="error-handling"></a>Fehlerbehandlung

Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf. Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite    |
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
|values|(boolean or string or number)|Optional. Ein 2-dimensionales Array der unformatierte Werte der Tabellenzeilen.|

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
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablerowcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
