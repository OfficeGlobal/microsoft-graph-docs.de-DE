---
title: Befehl Gerätestatus anfordern.
description: Rufen Sie den Status eines Befehls auf einem Gerät. Die vollständige Liste der Statuscodes finden Sie unter Liste der ActionStatus.
ms.openlocfilehash: 1e51d3b4366e87d9802518a50fe348d3ba0f250d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058021"
---
# <a name="get-device-command-status"></a>Befehl Gerätestatus anfordern.

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie den Status eines Befehls auf einem Gerät. Die vollständige Liste der Statuscodes finden Sie unter [Liste der ActionStatus](#list-of-actionstatus).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Nicht unterstützt    |
|Delegiert (persönliches Microsoft-Konto) | Device.Command    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile |Wert
|:----|:------|
|Authorization| Bearer {token}. Erforderlich. |
|Accept | application/json |

## <a name="response"></a>Antwort
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a>Liste der actionStatus

- Anfordern von / / Befehl erstellt wurde und wartet auf Verarbeitung
- SentToTarget, / / Befehl an das Gerät gesendet wurde
- ausführen, / / Zielgerät Bestätigung des Befehls bestätigt und ausgeführt wird
- abgeschlossen, / / Command Ausführung beendet
- FailedToSend, / / -Dienst konnte nicht auf das Zielgerät Befehl senden
- ExecutionFailed, / / Command fehlgeschlagen
- CommandDropped, / / Befehl vom Client gelöscht, wenn ConnectedStandby Gerät ist
- Abbrechen, / / Abbrechen des Befehls
- Abbrechen, / / den Befehl wird abgebrochen.
- abgebrochen, / / Befehl wurde abgebrochen
- Wiederholen, / / Dienst wird zum Senden von Befehl an Ziel wiederholen
- abgelaufen, / / Befehl Verarbeitung Ablaufzeit überschritten
- Fehler: / / Interner Fehler beim Ausführen des Befehls
- Benutzerdefinierte / / benutzerdefinierte Status

## <a name="example"></a>Beispiel

In diesem Beispiel benötigen Sie die ID des Geräts und die ID des Befehls, die zu einem Gerät ausgestellt wurde. Das Gerät ID wird zurückgegeben, beim Ausgeben eines GET-Anruf, um `/me/devices`, und rufen Sie der Befehl ID wird zurückgegeben, wenn einen Beitrag wie folgt auf `/me/devices/{id}/command`.

#### <a name="request"></a>Anforderung

Das folgende Beispiel zeigt die Antwort.

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Antwort

Das folgende Beispiel zeigt die Antwort.
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a>Abrufen der Befehl Nutzlast

Rufen Sie eine Antwort Nutzlast für eine bestimmte Aktion auf einem Gerät. Nutzlast Antwort wird beim Abfragen eines app-Service verwendet, für die Übermittlung von Daten zurück.


### <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Nicht unterstützt    |
|Delegiert (persönliches Microsoft-Konto) | Device.Command    |
|Anwendung | Nicht unterstützt |

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a>Anforderungsheader

| Kopfzeile |Wert
|:----|:------|
|Authorization| Bearer {token}. Erforderlich. |
|Accept | application/json |

### <a name="response"></a>Antwort
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a>Beispiel

In diesem Beispiel benötigen Sie die ID des Geräts und die ID des Befehls, die zu einem Gerät ausgestellt wurde. Rufen Sie das Gerät ID wird zurückgegeben, wenn einen GET ausstellen für `/me/devices`, und rufen Sie der Befehl ID wird zurückgegeben, wenn einen Beitrag wie folgt auf `/me/devices/{id}/command`.

#### <a name="request"></a>Anforderung

Das folgende Beispiel zeigt die Antwort.

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Antwort

Das folgende Beispiel zeigt die Antwort.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
