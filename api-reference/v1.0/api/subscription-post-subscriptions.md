---
title: Abonnement erstellen
description: Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden
localization_priority: Priority
ms.openlocfilehash: 07b2c055c49a79f1d9d3407ba8da5a5658766d20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889628"
---
# <a name="create-subscription"></a>Abonnement erstellen

Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden

## <a name="permissions"></a>Berechtigungen

Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Ressourcentyp/Element        | Berechtigung          |
|-----------------------------|---------------------|
| Kontakte                    | Contacts.Read       |
| Unterhaltungen               | Group.Read.All      |
| Ereignisse                      | Calendars.Read      |
| Nachrichten                    | Mail.Read           |
| Gruppen                      | Group.Read.All      |
| Benutzer                       | User.Read.All       |
| Laufwerk (OneDrive eines Benutzers)    | Files.ReadWrite     |
| Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke) | Files.ReadWrite.All |
|Sicherheitshinweis| SecurityEvents.ReadWrite.All |

 > **Hinweis:** Der Endpunkt /v1.0 kann Berechtigungen für die meisten Ressourcen. Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.

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

Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Abonnement](../resources/subscription.md) -Objekts.
Die `clientState` Feld ist optional.

##### <a name="resources-examples"></a>Beispiele für Ressourcen

Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:

| Ressourcentyp | Beispiele |
|:------ |:----- |
|Mail|me/mailfolders('inbox')/messages<br />me/messages|
|Kontakte|me/contacts|
|Kalender|me/events|
|Benutzer|users|
|Gruppen|Gruppen|
|Unterhaltungen|groups('*{id}*')/conversations|
|Laufwerke|me/drive/root|
|Sicherheitshinweis|Sicherheitshinweise /? $filter = Status Eq 'Neu'|

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

Das Abonnement Benachrichtigung Endpunkt (im angegebenen der `notificationUrl` -Eigenschaft) müssen Daten aneinander zur Reaktion auf eine Anforderung zur Überprüfung, wie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks#notification-endpoint-validation). Wenn die Überprüfung fehlschlägt, gibt die Anforderung an das Abonnement zu erstellen einer 400-Bad Request-Fehler zurück.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
