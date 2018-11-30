---
title: 'Arbeitsblatt: UsedRange'
description: Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.
ms.openlocfilehash: 424d8226a8f109242956b139670ed674ae50b43d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059600"
---
# <a name="worksheet-usedrange"></a>Arbeitsblatt: UsedRange

Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.
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
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a>Funktionsparameter
Stellen Sie in der Anforderungs-URL einen optionalen Abfrageparameter bereit.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|valuesOnly|Boolesch|Optional. Betrachtet nur Zellen mit Werten als verwendet (ignoriert die Formatierung).|

## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Arbeitsmappensitzungs-ID  | Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
