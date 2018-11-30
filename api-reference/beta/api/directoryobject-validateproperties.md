---
title: 'DirectoryObject: ValidateProperties'
description: Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht.  Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Erstellen** . Verwenden Sie zum Überprüfen von Eigenschaften einer vorhandenen Gruppe, die ValidateProperties-Funktion für Gruppen.
ms.openlocfilehash: 82592eff14829fdd8ae1d74c87f43402a3938adf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059590"
---
# <a name="directoryobject-validateproperties"></a>DirectoryObject: ValidateProperties

Überprüfen Sie, ob eine Office 365-Gruppe Display Name oder die e-Mail-Spitzname naming Richtlinien entspricht.  Clients können mithilfe der API bestimmen, ob ein Anzeigename oder e-Mail-Spitzname ist gültig, bevor Sie versuchen, eine Office 365-Gruppe zu **Erstellen** . Zum Überprüfen von Eigenschaften einer vorhandenen Gruppe, verwenden Sie die [Funktion ValidateProperties](group-validateproperties.md) für Gruppen.

Für die Namen und e-Mail-Spitzname Anzeigeeigenschaften werden die folgenden Überprüfungen ausgeführt: 
1. Überprüfen Sie das Präfix und Suffix Richtlinie zum Benennen
2. Überprüfen Sie die benutzerdefinierten gesperrten Wörter-Richtlinie
3. Überprüfen Sie die e-Mail-Nachricht Spitzname eindeutig ist.

Diese API zurückgegeben mit ersten Fehler. Wenn mehrere Überprüfungen eine oder mehrere Eigenschaften ein Fehler auftritt, wird nur die-Eigenschaft mit den ersten Validierungsfehler zurückgegeben. Sie können jedoch überprüft e-Mail-Spitznamen und den Anzeigenamen und eine Auflistung von Validierungsfehlern empfangen, wenn Sie nur das Präfix und Suffix Richtlinie zum Benennen überprüfen.

## <a name="prerequisites"></a>Voraussetzungen

Die folgende **Berechtigung** ist erforderlich, um diese API ausführen: *Group.Read.All*

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
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
|entityType|String| `Group`ist der einzige unterstützte Entitätstyp an. |
|displayName|String| Der Anzeigename der Gruppe zu überprüfen. Die Eigenschaft ist nicht einzeln erforderlich. Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich. |
|mailNickname|String| Die e-Mail-Spitzname der Gruppe zu überprüfen. Die Eigenschaft ist nicht einzeln erforderlich. Mindestens eine Eigenschaft (DisplayName oder MailNickname) ist jedoch erforderlich. |
|onBehalfOfUserId|Guid| Die Objekt-ID des Benutzers zum imitieren beim Aufrufen der API. Die Überprüfungsergebnisse werden für die OnBehalfOfUserId Attribute und Rollen. |

## <a name="response"></a>Antwort

Bei erfolgreicher und es liegen keine Validierungsfehler, die Methode gibt `204 No Content` Antwortcode. Es gibt keine Suchzeichenfolge im Antworttext zurück.

Wenn die Anforderung ungültig ist, gibt die Methode `400 Bad Request` Antwortcode. Eine Fehlermeldung mit Details über die ungültige Anforderung wird in der Antworttext zurückgegeben.

Wenn ein Gültigkeitsprüfungsfehler vorhanden ist, gibt die Methode `422 Unprocessable Entity` Antwortcode. In den Antworttext wird eine Fehlermeldung angezeigt und eine Auflistung von Fehlerdetails zurückgegeben.

## <a name="examples"></a>Beispiele

Dies ist ein Beispiel für eine Anforderung erfolgreicher Überprüfung.

### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

Dies ist ein Beispiel für eine Anforderung mit Überprüfungsfehlern.

### <a name="request"></a>Anforderung
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Antwort
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
