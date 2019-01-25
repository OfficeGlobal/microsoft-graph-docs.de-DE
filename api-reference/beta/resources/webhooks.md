---
title: Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern
description: Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Einzelheiten, einschließlich das Abonnieren und behandeln eingehende Benachrichtigungen Set finden Sie unter Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 02ab18d3fa8980211a4937433ad1616b0629bf8c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526214"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Informationen zum Abonnieren und behandeln eingehende Benachrichtigungen finden Sie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks), einschließlich.

Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

- Nachrichten
- Ereignisse
- Kontakte
- Benutzer
- Gruppen
- Gruppenunterhaltungen
- Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke
- Persönlichen OneDrive-Ordnern des Benutzers
- Sicherheitswarnungen

## <a name="permissions"></a>Berechtigungen

In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.

| Berechtigungstyp                        | Unterstützten Ressourcentypen                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegiert – Geschäfts-, Schul- oder Unikonto     | [wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][], [Benachrichtigung][] |
| Delegiert – persönliches Microsoft-Konto | [wenden Sie sich an][], [Laufwerk][], [Ereignis][], [Nachricht][]                                        |
| Anwendung                            | [wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][], [Benachrichtigung][] |

## <a name="see-also"></a>Siehe auch

- [Abonnementressourcentyp](subscription.md)
- [Liste von Abonnements](../api/subscription-list.md)
- [Abonnement abrufen](../api/subscription-get.md)
- [Abonnement erstellen](../api/subscription-post-subscriptions.md)
- [Update subscription](../api/subscription-update.md)
- [Delete subscription](../api/subscription-delete.md)

[Kontakt]: ./contact.md
[Unterhaltung]: ./conversation.md
[Laufwerk]: ./drive.md
[Ereignis]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
Alert
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
