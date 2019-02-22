---
title: Abonnement aktualisieren
description: Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1bf693fb8551db916807570459d9658fa02665f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167802"
---
# <a name="update-subscription"></a>Abonnement aktualisieren

Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.

Abonnements laufen nach einer vom Ressourcentyp unterschiedlichen Zeitspanne ab. Um fehlende Benachrichtigungen zu vermeiden, sollte eine APP Ihre Abonnements vor Ablauf des Gültigkeitszeitraums verlängern. Weitere Informationen finden Sie unter [Abonnement](../resources/subscription.md) für die maximale Länge eines Abonnements für die einzelnen Ressourcentypen.

## <a name="permissions"></a>Berechtigungen

Abhängig von der angeforderten Ressource und dem Berechtigungstyp (Delegierte oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die am wenigsten privilegierten Berechtigungen zum Aufrufen dieser API. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
|[Kontakt](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (persönliche OneDrive des Benutzers) | Nicht unterstützt | Files.ReadWrite | Nicht unterstützt |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Nicht unterstützt | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Nicht unterstützt | Group.Read.All |
|[Gruppenunterhaltung](../resources/conversation.md) | Group.Read.All | Nicht unterstützt | Nicht unterstützt |
|[Nachricht](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[Sicherheitswarnung](../resources/alert.md) | SecurityEvents.ReadWrite.All | Nicht unterstützt | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive-und Outlook-Elemente. Die Einschränkungen gelten für das Erstellen und Verwalten von Abonnements (erhalten, aktualisieren und Löschen von Abonnements).

- In persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner in diesem Laufwerk abonnieren. In OneDrive for Business können Sie nur den Stammordner abonnieren. Benachrichtigungen werden für die angeforderten Arten von Änderungen im abonnierten Ordner oder in einer beliebigen Datei, einem Ordner oder einem anderen driveItem-Objekt in der Hierarchie gesendet. Sie können keine **Laufwerks** -oder **driveItem** -Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.

- In Outlook unterstützt die Delegierte Berechtigung das Abonnieren von Elementen in Ordnern nur im Postfach des angemeldeten Benutzers. Das kann beispielsweise nicht die Delegierte Berechtigung Calendars. Read verwenden, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.
- So abonnieren Sie Änderungsbenachrichtigungen für Outlook-Kontakte,-Ereignisse oder-Nachrichten in _freigegebenen oder Delegierten_ Ordnern:

  - Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen an Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.
  - Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts. Read. Shared, Calendars. Read. Shared, Mail. Read. Shared und ihre Pendants für Lese-/Schreibzugriff), da Sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder Delegierten Ordnern **nicht** unterstützen.


## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
