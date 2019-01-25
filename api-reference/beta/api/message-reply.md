---
title: 'message: reply'
description: 'Antwort an den Absender einer Nachricht, einen Kommentar hinzufügen oder ändern aktualisierbaren Eigenschaften alle in eine **Antwort** Anruf. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6461d9735459ff9cf956820b00bb61a4d42d1ec0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519010"
---
# <a name="message-reply"></a>message: reply

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Antwortet dem Absender einer Nachricht, fügt einen Kommentar hinzu oder ändert aktualisierbare Eigenschaften in einem **reply**-Aufruf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.

Alternativ können Sie zunächst [den Entwurf einer Antwortnachricht erstellen](../api/message-createreply.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Eigenschaften der Nachricht, und die Antwort zu [Senden](../api/message-send.md) .

**Hinweis**

- Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter. Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.
- Wenn die **ReplyTo** -Eigenschaft angegeben wird, in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), sollten Sie in **ReplyTo** und nicht der Empfänger in der Eigenschaft **aus** die Antwort an den Empfänger senden. 


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Mail.Send    |
|Delegiert (persönliches Microsoft-Konto) | Mail.Send    |
|Anwendung | Mail.Send |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type | string  | Die Art der Daten im Textkörper einer Entität. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|comment|String|Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.|
|message|[Nachricht](../resources/message.md)|Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
Das folgende Beispiel enthält einen Kommentar und Antwortnachricht einen Empfänger hinzugefügt.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
