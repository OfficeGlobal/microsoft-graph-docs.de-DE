---
title: Abonnement erstellen
description: Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Daten in einer Microsoft Graph-Ressource geändert werden.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140166"
---
# <a name="create-subscription"></a>Abonnement erstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn der angeforderte Änderungstyp für die angegebene Ressource in Microsoft Graph auftritt.

## <a name="permissions"></a>Berechtigungen

Das Erstellen eines Abonnements erfordert Lesebereich für die Ressource. Wenn Sie beispielsweise Benachrichtigungen zu Nachrichten erhalten möchten, benötigt Ihre `Mail.Read` APP die Berechtigung. 
 
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

- In persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner in diesem Laufwerk abonnieren. In OneDrive for Business können Sie nur den Stammordner abonnieren. Benachrichtigungen werden für die angeforderten Änderungstypen im abonnierten Ordner oder für eine beliebige Datei, einen Ordner oder eine andere **driveItem** -Instanz in der Hierarchie gesendet. Sie können keine **Laufwerks** -oder **driveItem** -Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.

- In Outlook unterstützt die Delegierte Berechtigung das Abonnieren von Elementen in Ordnern nur im Postfach des angemeldeten Benutzers. Das kann beispielsweise nicht die Delegierte Berechtigung Calendars. Read verwenden, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.
- So abonnieren Sie Änderungsbenachrichtigungen für Outlook-Kontakte,-Ereignisse oder-Nachrichten in _freigegebenen oder Delegierten_ Ordnern:

  - Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen an Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.
  - Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts. Read. Shared, Calendars. Read. Shared, Mail. Read. Shared und ihre Pendants für Lese-/Schreibzugriff), da Sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder Delegierten Ordnern **nicht** unterstützen.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Geben Sie im Anforderungstext eine JSON-Darstellung des [Subscription](../resources/subscription.md) -Objekts an.
Das `clientState` Feld ist optional.

In dieser Beispielanforderung wird ein Abonnement für Benachrichtigungen über neue e-Mails erstellt, die von dem derzeit signierten Benutzer empfangen werden.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

Die folgenden Werte gelten für die Resource-Eigenschaft:

| Ressourcentyp | Beispiele |
|:------ |:----- |
|Mail|me/mailfolders('inbox')/messages<br />me/messages|
|Kontakte|me/contacts|
|Kalender|me/events|
|Benutzer|users|
|Gruppen|Gruppen|
|Unterhaltungen|groups('*{id}*')/conversations|
|Laufwerke|me/drive/root|
|Sicherheitswarnung|Sicherheit/Warnungen? $filter = Status-EQ ' neu '|

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>Endpunktprüfung für Benachrichtigungen

Der Abonnement Benachrichtigungs Endpunkt (in der `notificationUrl` Eigenschaft angegeben) muss auf eine Validierungs Anforderung reagieren können, wie unter [Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten](/graph/webhooks#notification-endpoint-validation)beschrieben. Wenn die Validierung fehlschlägt, gibt die Anforderung zum Erstellen des Abonnements einen Fehler vom 400 unGültigen Anforderung zurück.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
