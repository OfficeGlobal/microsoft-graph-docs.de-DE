---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9fa5a60bbb00bb7d15ae14a0b76235a5629f2c42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140453"
---
# <a name="delete-subscription"></a>Abonnement löschen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit dieser API können Sie Abonnements löschen.

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
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
