---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Aktualisieren eines Eintrags in einer SharePoint-Liste
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f80f2607e953ba760893170366179f6751d9665d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481993"
---
# <a name="update-an-item-in-a-list"></a>Element in einer Liste aktualisieren

Aktualisieren Sie die Eigenschaften in einem **[listItem][]**.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name       | Wert | Beschreibung
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht aktualisiert.


## <a name="request-body"></a>Anforderungstext

Geben Sie im Textbereich eine JSON-Darstellung von einem [FieldValueSet][] an, um die Felder für die Aktualisierung anzugeben.

## <a name="example"></a>Beispiel

Dies ist ein Beispiel für die Aktualisierung der Felder Farbe und Menge Felder des Listenelements mit neuen Werten.
Alle anderen Werte des listItem bleiben unberührt. 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird ein [fieldValueSet][]-Objekt im Antworttext des aktualisierten Listenelements zurückgegeben.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
