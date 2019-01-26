---
title: Erweiterte einwertige Eigenschaft erstellen
description: 'Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource. '
localization_priority: Normal
ms.openlocfilehash: 6a9ddee699cac0e11a5656fc12174a9d4fb610c3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575447"
---
# <a name="create-single-value-extended-property"></a>Erweiterte einwertige Eigenschaft erstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource. 

Die folgenden Benutzerressourcen werden unterstützt:

- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 
- [Ereignis](../resources/event.md)
- [mailFolder](../resources/mailfolder.md)
- [Nachricht](../resources/message.md)
- [Outlook-Aufgabe](../resources/outlooktask.md)
- [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md)

Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:

- [calendar](../resources/calendar.md)-Ressourcen für Gruppen
- [event](../resources/event.md)-Ressourcen für Gruppen
- [post](../resources/post.md)-Ressourcen für Gruppen 

Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.

## <a name="permissions"></a>Berechtigungen
Erstellen Sie je nach der Ressource in die erweiterte Eigenschaft und die Berechtigung geben (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
| [Kalender](../resources/calendar.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [Kontakt](../resources/contact.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [contactFolder](../resources/contactfolder.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [event](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite |  Calendars.ReadWrite|
| [calendar](../resources/calendar.md)-Ressourcen für Gruppen | Group.ReadWrite.All | Nicht unterstützt | Nicht unterstützt |
| [event](../resources/event.md)-Ressourcen für Gruppen | Group.ReadWrite.All | Nicht unterstützt | Nicht unterstützt |
| [post](../resources/post.md)-Ressourcen für Gruppen | Group.ReadWrite.All | Nicht unterstützt | Nicht unterstützt |
| [mailFolder](../resources/mailfolder.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite |
| [message](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite |
| [Outlook-Aufgabe](../resources/outlooktask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Nicht unterstützt |
| [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md) | Tasks.ReadWrite | Tasks.ReadWrite | Nicht unterstützt |
 
## <a name="http-request"></a>HTTP-Anforderung
Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.

Um eine oder mehrere erweiterte Eigenschaften in einer _neuen_ Instanz der Ressource zu erstellen, verwenden Sie die gleiche REST-Anforderung als die Instanz erstellt und enthalten Sie die Eigenschaften für die neue Ressource Instanz _und erweiterte Eigenschaft_ im Textkörper Anforderung.
Beachten Sie, dass einige Ressourcen in mehr als eine Möglichkeit der Erstellung unterstützt. Weitere Informationen zum Erstellen dieser Ressourceninstanzen, finden Sie unter den entsprechenden Themen für die Erstellung einer [Nachricht](../resources/message.md), [MailFolder](../api/user-post-mailfolders.md), [Ereignis](../api/user-post-events.md), [Kalender](../api/user-post-calendars.md), [wenden Sie sich an](../api/user-post-contacts.md), [ContactFolder](../api/user-post-contactfolders.md), [Outlook-Aufgabe](../resources/outlooktask.md), [ Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md), [Gruppe Ereignis](../api/group-post-events.md)und [Gruppe Post](../resources/post.md). 
 
So sieht die Syntax der Anforderungen aus: 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.

**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Wert |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie einen JSON Rumpf jedes [SingleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) -Objekts in die **SingleValueLegacyExtendedProperty** Collection-Eigenschaft einer Instanz der Ressource.

|**Eigenschaft**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|singleValueLegacyExtendedProperty|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung| Ein Array aus erweiterten mehrwertigen Eigenschaften. |
|id|String|Geben Sie für jede Eigenschaft in der Auflistung **SingleValueLegacyExtendedProperty** diese Option, damit die Eigenschaft ermitteln. Es muss eine der unterstützten Formate folgen. Weitere Informationen finden Sie unter [Outlook erweiterte Eigenschaften (Übersicht)](../resources/extended-properties-overview.md) . Erforderlich.|
|Wert|string|Geben Sie für jede Eigenschaft in der Auflistung **SingleValueLegacyExtendedProperty** Wert der Eigenschaft. Erforderlich.|

Geben Sie beim Erstellen einer erweiterten Eigenschaft in eine _neue_ Instanz der Ressource, zusätzlich zu der neuen **SingleValueLegacyExtendedProperty** -Auflistung eine JSON-Darstellung der Ressourceninstanz (d. h., eine [Nachricht](../resources/message.md), [mailFolder ](../resources/mailfolder.md), [Ereignis](../resources/event.md)usw..)

## <a name="response"></a>Antwort

#### <a name="response-code"></a>Antwortcode
Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.

Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück. 


#### <a name="response-body"></a>Antworttext

Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/singlevaluelegacyextendedproperty-get.md).

Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ [Gruppenbeitrag](../resources/post.md) durch Antwort auf einen Thread oder Beitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft.



## <a name="example"></a>Beispiel
##### <a name="request-1"></a>Anforderung 1

Im erste Beispiel erstellt ein neues Ereignis und eine erweiterte Einzelwert-Eigenschaft in der gleichen POST-Operation. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis aufnehmen möchten, enthält der Anforderungstext **SingleValueLegacyExtendedProperty** -Auflistung, die eine erweiterte einwertig-Eigenschaft und die folgenden für die Eigenschaft enthält:

- **ID** Gibt den Eigenschaftstyp als `String`, die GUID und die `Fun`-Eigenschaft an.
- **Wert** Gibt `Food` als den Wert der `Fun`-Eigenschaft an. 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueLegacyExtendedProperty": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a>Antwort 1

Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user-post-events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.

Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/singlevaluelegacyextendedproperty-get.md).


****

##### <a name="request-2"></a>Anforderung 2

Im zweite Beispiel erstellt einen Single-Wert, erweiterte Eigenschaft für die angegebene vorhandene Nachricht. Mit der erweiterten Eigenschaft ist das einzige Element im Array **SingleValueLegacyExtendedProperty** . Textkörper der Anforderung umfasst folgende für die erweiterte Eigenschaft:
- **ID** Gibt den Eigenschaftstyp als `String`, die GUID und die `Color`-Eigenschaft an.
- **Wert** Gibt `Green` als den Wert der `Color`-Eigenschaft an.

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueLegacyExtendedProperty": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a>Antwort 2

Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message-update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.

Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/singlevaluelegacyextendedproperty-get.md).

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

