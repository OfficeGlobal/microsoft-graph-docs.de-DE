---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: f2a1088ac6f84d236aec64fad6e0fd0d9d21e473
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156469"
---
# <a name="get-subscription"></a>Abonnement abrufen

Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.

## <a name="permissions"></a>Berechtigungen

Abhängig von der Ressource und dem angeforderten Berechtigungstyp (delegiert oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die niedrigste Berechtigung, die zum Aufrufen dieser API erforderlich ist. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
|[Kontakt](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (persönliche OneDrive-Umgebung eines Benutzers) | Nicht unterstützt | Files.ReadWrite | Nicht unterstützt |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Nicht unterstützt | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Nicht unterstützt | Group.Read.All |
|[Gruppenunterhaltung](../resources/conversation.md) | Group.Read.All | Nicht unterstützt | Nicht unterstützt |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[security alert](../resources/alert.md) | SecurityEvents.ReadWrite.All | Nicht unterstützt | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive- und Outlook-Elemente. Die Einschränkungen gelten sowohl für die Erstellung als auch für die Verwaltung von Abonnements (Abrufen, Aktualisieren und Löschen von Abonnements).

- Auf dem persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner auf diesem Laufwerk abonnieren. Bei OneDrive for Business können Sie nur den Stammordner abonnieren. Benachrichtigungen werden für die angeforderten Arten von Änderungen am abonnierten Ordner bzw. an einer Datei, einem Ordner oder anderen "driveItem"-Objekten in seiner Hierarchie gesendet. Sie können keine **drive**- oder **driveItem**-Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.

- In Outlook unterstützt die delegierte Berechtigung das Abonnieren von Elementen ausschließlich in Ordnern, die sich im Postfach des angemeldeten Benutzers befinden. Das bedeutet, dass Sie beispielsweise nicht die delegierte Berechtigung "Calendars.Read" verwenden können, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.
- So abonnieren Sie Änderungsbenachrichtigungen über Outlook-Kontakte, -Ereignisse oder -Nachrichten in _freigegebenen oder delegierten Ordnern_:

  - Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen von Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.
  - Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared und ihre read/write-Entsprechungen), da sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder delegierten Ordnern **nicht** unterstützen.
 

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
