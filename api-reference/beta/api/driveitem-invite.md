---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Senden einer Einladung für den Zugriff auf ein Element
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1e02af913702aace46a5e3ca2f2e2650a2c7839e
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676975"
---
# <a name="send-a-sharing-invitation"></a>Freigabeeinladung senden

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sendet eine Freigabeeinladung für ein **DriveItem**-Element. Eine Freigabeeinladung stellt Berechtigungen für Empfänger bereit und sendet optional eine E-Mail-Nachricht an den Empfänger, um diesen über die Freigabe in Kenntnis zu setzen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite, Files.ReadWrite.All    |
|Anwendung | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| Parameter        | Typ                                            | Beschreibung                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| recipients       | Collection([DriveRecipient](../resources/driverecipient.md)) | Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.                                            |
| message          | String                                          | Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen. |
| requireSignIn    | Boolesch                                         | Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.            |
| sendInvitation   | Boolean                                         | Gibt an, ob eine E-Mail oder ein Beitrag generiert (falsch) oder ob nur die Berechtigung erstellt (true) wurde.            |
| roles            | Collection(String)                              | Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.                         |
| expirationDateTime | DateTimeOffset                       | Geben Sie den DateTime-Datentyp an, nach dem die Berechtigung abläuft. Verfügbar unter OneDrive for Business-, SharePoint-und Premium-persönlichen OneDrive-Konten.
| password           | Zeichenfolge                         | Das auf der Einladung vom Ersteller festgelegte Kennwort. Nur optional und OneDrive Personal

## <a name="example"></a>Beispiel

In diesem Beispiel wird eine Einladung zur Freigabe an einen Benutzer mit der E-Mail-Adresse "ryan@contoso.org" versandt, in der dieser über eine Datei für die Zusammenarbeit benachrichtigt wird.
Die Einladung gewährt Ryan Lese-/ Schreibzugriff auf die Datei.

### <a name="http-request"></a>HTTP-Anforderung

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.

<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a>Partielle Erfolgsantwort

Bei der Einladung mehrerer Empfänger ist es möglich, dass die Benachrichtigung für einige erfolgreich ist und für andere Benutzer fehlschlägt.
In diesem Fall gibt der Dienst eine teilweisen Erfolgsantwort mit einem HTTP-Statuscode von 207 zurück.
Wenn ein teilweiser Erfolg zurückgegeben wird, enthält die Antwort für jeden Fehler `error` haften Empfänger ein Objekt mit Informationen darüber, was schief gelaufen ist und wie es behoben werden kann.

Hier ist ein Beispiel für die partielle Antwort.  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a>SendNotification-Fehler
Im folgenden finden Sie einige zusätzliche Fehler, die Ihre APP in den geschachtelten `innererror` Objekten auftreten kann, wenn beim Senden der Benachrichtigung ein Fehler auftritt. Apps müssen diese nicht verarbeiten.

| Code                           | Beschreibung
|:-------------------------------|:--------------------------------------------------------------------------------------
| accountVerificationRequired    | Die Kontoüberprüfung ist erforderlich, um das Senden von Benachrichtigungen aufzuheben.
| hipCheckRequired               | Sie müssen die HIP (Host Intrusion Prevention)-Überprüfung lösen, um das Senden von Benachrichtigungen aufzuheben.
| exchangeInvalidUser            | Das Postfach des aktuellen Benutzers wurde nicht gefunden.
| exchangeOutOfMailboxQuota      | Außerhalb des Kontingents.
| exchangeMaxRecipients          | Die maximale Anzahl von Empfängern, die gleichzeitig gesendet werden können, wurde überschritten.

>**Hinweis:** Der Dienst kann neue Fehlercodes hinzufügen oder die Rückgabe von alten Dateien jederzeit beenden.

## <a name="remarks"></a>Hinweise

* [Laufwerke](../resources/drive.md) mit dem**driveType**`personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.
* Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration-values).

## <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
