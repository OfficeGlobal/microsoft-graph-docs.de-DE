---
title: Abonnement erstellen
description: Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 6d06e230dd85aadaa4d2b3a4f851b339b34793eb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157694"
---
# <a name="create-subscription"></a>Abonnement erstellen

Abonniert eine Listener-Anwendung, um Benachrichtigungen zu erhalten, wenn die angeforderte Art von Änderungen an der angegebenen Ressource in Microsoft Graph auftritt.

## <a name="permissions"></a>Berechtigungen

 Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. 
 
 Abhängig von der Ressource und dem angeforderten Berechtigungstyp (delegiert oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die niedrigste Berechtigung, die zum Aufrufen dieser API erforderlich ist. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
|[contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (persönliche OneDrive-Umgebung eines Benutzers) | Nicht unterstützt | Files.ReadWrite | Nicht unterstützt |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Nicht unterstützt | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Nicht unterstützt | Group.Read.All |
|[group conversation](../resources/conversation.md) | Group.Read.All | Nicht unterstützt | Nicht unterstützt |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[security alert](../resources/alert.md) | SecurityEvents.ReadWrite.All | Nicht unterstützt | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive- und Outlook-Elemente. Die Einschränkungen gelten sowohl für die Erstellung als auch für die Verwaltung von Abonnements (Abrufen, Aktualisieren und Löschen von Abonnements).

- Auf dem persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner auf diesem Laufwerk abonnieren. Bei OneDrive for Business können Sie nur den Stammordner abonnieren. Benachrichtigungen werden für die angeforderten Arten von Änderungen am abonnierten Ordner bzw. an einer Datei, einem Ordner oder anderen **driveItem**-Instanzen in seiner Hierarchie gesendet. Sie können keine **drive**- oder **driveItem**-Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.

- In Outlook unterstützt die delegierte Berechtigung das Abonnieren von Elementen ausschließlich in Ordnern, die sich im Postfach des angemeldeten Benutzers befinden. Das bedeutet, dass Sie beispielsweise nicht die delegierte Berechtigung "Calendars.Read" verwenden können, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.
- So abonnieren Sie Änderungsbenachrichtigungen über Outlook-Kontakte, -Ereignisse oder -Nachrichten in _freigegebenen oder delegierten Ordnern_:

  - Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen von Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.
  - Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared und ihre read/write-Entsprechungen), da sie **nicht** das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder delegierten Ordnern unterstützen. 


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

Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

Geben Sie im Anforderungstext eine JSON-Darstellung des [subscription](../resources/subscription.md)-Objekts an.
Das `clientState`-Feld ist optional.

##### <a name="resources-examples"></a>Beispiele für Ressourcen

Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:

| Ressourcentyp | Beispiele |
|:------ |:----- |
|Mail|me/mailfolders('inbox')/messages<br />me/messages|
|Kontakte|me/contacts|
|Kalender|me/events|
|Benutzer|users|
|Gruppen|groups|
|Unterhaltungen|groups('*{id}*')/conversations|
|Laufwerke|me/drive/root|
|Sicherheitswarnung|security/alerts?$filter=status eq ‘New’|

##### <a name="response"></a>Reaktion

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

Der Endpunkt der Abonnementbenachrichtigung (angegeben in der Eigenschaft `notificationUrl`) muss in der Lage sein, auf eine Validierungsanforderung zu reagieren, wie unter [Einrichten von Benachrichtigungen für Änderungen an Benutzerdaten](/graph/webhooks#notification-endpoint-validation) beschrieben. Wenn die Validierung fehlschlägt, gibt die Anforderung zur Erstellung des Abonnements einen "400 Bad Request"-Fehler zurück.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
