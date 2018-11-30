---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Versenden einer Einladung für den Zugriff auf ein Element
ms.openlocfilehash: db089fcd0a3f948d8e43f366a4e6674c2505fa2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016978"
---
# <a name="send-a-sharing-invitation"></a>Freigabeeinladung senden

Sendet eine Einladung zur Freigabe für eine **DriveItem**.
Eine Einladung zur Freigabe Berechtigungen an die Empfänger enthält, und sendet sie optional eine e-Mail mit einem [Link Freigabe][].

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

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| Parameter        | Typ                           | Beschreibung
|:-----------------|:-------------------------------|:-------------------------
| recipients       | Collection([DriveRecipient][]) | Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.
| message          | String                         | Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.
| requireSignIn    | Boolean                        | Gibt an, ob der Empfänger der Einladung zur Anmeldung an das freigegebene Element anzeigen erforderlich ist.
| sendInvitation   | Boolean                        | Bei true wird eine [Freigabe Link][] an den Empfänger gesendet. Andernfalls wird eine Berechtigung erteilt, direkt und ohne eine Benachrichtigung sendet.
| roles            | Collection(String)             | Geben Sie die Rollen, die an die Empfänger, der die Einladung zur Freigabe erteilt werden.

## <a name="example"></a>Beispiel

In diesem Beispiel sendet eine freigabeeinladung für einen Benutzer mit e-Mail-Adresse "ryan@contoso.com" mit einer Meldung über eine Datei wird arbeiteten an.
Die Einladung gewährt Ryan Lese-/ Schreibzugriff auf die Datei.

### <a name="http-request"></a>HTTP-Anforderung

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
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


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[Freigeben von link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
