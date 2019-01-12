---
title: Erstellen Sie und senden Sie eine Benachrichtigung
description: 'Erstellen Sie und senden Sie eine Benachrichtigung für einen Benutzer über Microsoft Graph. Die Benachrichtigung wird in der Microsoft Graph-Benachrichtigung feed Store gespeichert und an alle Geräte-Endpunkten, bei denen der Benutzer, in angemeldet ist allen app-Clients gesendet.  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: d8258e0da04f199a0f40bdb2a2ec85e01d5d5faf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975932"
---
# <a name="create-and-send-a-notification"></a>Erstellen Sie und senden Sie eine Benachrichtigung
> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie und senden Sie eine Benachrichtigung für einen Benutzer über Microsoft Graph. Die Benachrichtigung wird in der Microsoft Graph-Benachrichtigung feed Store gespeichert und an alle Geräte-Endpunkten, bei denen der Benutzer, in angemeldet ist allen app-Clients gesendet.  
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Notifications.ReadWrite.CreatedByApp    |
|Delegiert (persönliches Microsoft-Konto) | Notifications.ReadWrite.CreatedByApp    |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Anforderungsheader
|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|Authorization | string |Der Authorization-Header wird verwendet, um die Anmeldeinformationen des Anrufers zu übergeben. Bearer {Token}. Erforderlich.  |
## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Benachrichtigung](../resources/projectrome-notification.md) .

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode die `201 Created` Antwortcode, der angibt, dass die Benachrichtigung erfolgreich erstellt und gespeichert wurde. 
## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


