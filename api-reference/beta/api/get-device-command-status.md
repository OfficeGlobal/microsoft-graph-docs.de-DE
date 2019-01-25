---
title: Befehl Gerätestatus anfordern.
description: Rufen Sie den Status eines Befehls auf einem Gerät. Die vollständige Liste der Statuscodes finden Sie unter Liste der ActionStatus.
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510113"
---
# <a name="get-device-command-status"></a>Befehl Gerätestatus anfordern.

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|Annehmen | application/json |

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
|Annehmen | application/json |

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
