---
title: Tabelle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Tabellenobjekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: df975d13ddc97c0c6b592d02d61a978c5a0db732
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919813"
---
# <a name="update-table"></a>Tabelle aktualisieren

Dient zum Aktualisieren der Eigenschaften des Tabellenobjekts.
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
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a>Optionale Anforderungsheader
| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Arbeitsmappensitzungs-ID  | Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|string|Der Name der Tabelle.|
|showHeaders|boolean|Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.|
|showTotals|boolean|Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.|
|style|string|Konstanter Wert, der das Tabellenformat darstellt. Die möglichen Werte sind: TableStyleLight1 bis TableStyleLight21 TableStyleMedium1 bis TableStyleMedium28 TableStyleStyleDark1 bis TableStyleStyleDark11. Eine benutzerdefinierte benutzerdefinierte Formatvorlage in der Arbeitsmappe vorhanden kann auch angegeben werden.|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookTable](../resources/table.md) -Objekt aus der Antwort.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
