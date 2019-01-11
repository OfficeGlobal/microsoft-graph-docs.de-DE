---
title: 'Gruppe: ValidateProperties'
description: Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht. Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Aktualisieren** . Verwenden Sie zum Überprüfen von Eigenschaften vor dem Erstellen einer Gruppe, die ValidateProperties-Funktion für Directory-Objekte.
localization_priority: Normal
ms.openlocfilehash: 0ffdf44f687ad047d952e00c268239432244006d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833901"
---
# <a name="group-validateproperties"></a>Gruppe: ValidateProperties

Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht. Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Aktualisieren** . Überprüfen vor dem Erstellen einer Gruppe von Eigenschaften, verwenden Sie die [ValidateProperties-Funktion](directoryobject-validateproperties.md) für Directory-Objekte.

Für die Namen und e-Mail-Spitzname Anzeigeeigenschaften werden die folgenden Überprüfungen ausgeführt: 
1. Überprüfen Sie das Präfix und Suffix Richtlinie zum Benennen
2. Überprüfen Sie die benutzerdefinierten gesperrten Wörter-Richtlinie

Diese API zurückgegeben mit ersten Fehler. Wenn mehrere Überprüfungen eine oder mehrere Eigenschaften ein Fehler auftritt, wird nur die-Eigenschaft mit den ersten Validierungsfehler zurückgegeben. Sie können jedoch überprüft e-Mail-Spitznamen und den Anzeigenamen und eine Auflistung von Validierungsfehlern empfangen, wenn Sie nur das Präfix und Suffix Richtlinie zum Benennen überprüfen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.Read.All, Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a>Anforderungsheader

| Name           | Beschreibung      |
|:---------------|:-----------------|
| Authorization  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|Zeichenfolge| Der Anzeigename der Gruppe zu überprüfen. Die Eigenschaft ist nicht einzeln erforderlich. Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich. |
|mailNickname|Zeichenfolge| Die e-Mail-Spitzname der Gruppe zu überprüfen. Die Eigenschaft ist nicht einzeln erforderlich. Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich. |
|onBehalfOfUserId|Guid| Die Objekt-ID des Benutzers zum imitieren beim Aufrufen der API. Die Überprüfungsergebnisse werden für die OnBehalfOfUserId Attribute und Rollen. |

## <a name="response"></a>Antwort
Bei erfolgreicher und es liegen keine Validierungsfehler, die Methode gibt `204 No Content` Antwortcode. Es gibt keine Suchzeichenfolge im Antworttext zurück.

Wenn die Anforderung ungültig ist, gibt die Methode `400 Bad Request` Antwortcode. Eine Fehlermeldung mit Details über die ungültige Anforderung wird in der Antworttext zurückgegeben.

Wenn ein Gültigkeitsprüfungsfehler vorhanden ist. Gibt die Methode `422 Unprocessable Entity` Antwortcode. In den Antworttext wird eine Fehlermeldung angezeigt und eine Auflistung von Fehlerdetails zurückgegeben.

## <a name="examples"></a>Beispiele

Dies ist ein Beispiel für eine Anforderung erfolgreicher Überprüfung.

### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

Dies ist ein Beispiel für eine Anforderung mit Überprüfungsfehlern.

### <a name="request"></a>Anforderung
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>Antwort
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
