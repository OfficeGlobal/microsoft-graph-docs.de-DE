---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Versenden einer Einladung für den Zugriff auf ein Element"
ms.openlocfilehash: 5be2060c190434c4b9d587d20fe68d69786b3aa5
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="send-a-sharing-invitation"></a>Freigabeeinladung senden

Sendet eine Freigabeeinladung für ein **DriveItem**-Element. Eine Freigabeeinladung stellt Berechtigungen für Empfänger bereit und sendet optional eine E-Mail-Nachricht an den Empfänger, um diesen über die Freigabe in Kenntnis zu setzen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

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
| requireSignIn    | Boolean                                         | Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.            |
| sendInvitation   | Boolean                                         | Gibt an, ob eine E-Mail oder ein Beitrag generiert (falsch) oder ob nur die Berechtigung erstellt (true) wurde.            |
| roles            | Collection(String)                              | Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.                         |

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
  "roles": [ "write" ]
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a>Hinweise

* [Laufwerke](../resources/drive.md) mit dem**driveType**`personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.
* Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration).

## <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].


[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->