---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c73f01a65a2b81bfa34818f9a7a96f754501bd65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163469"
---
# <a name="get-subscription"></a>Abonnement abrufen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.

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
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:-----|:-----------|
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
GET https://graph.microsoft.com/beta/subscriptions/{id}
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
