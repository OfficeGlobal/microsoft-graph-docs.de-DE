---
title: Verwenden der Microsoft Graph-API zum Abrufen von Änderungsbenachrichtigungen
description: Die Microsoft Graph-REST-API verwendet einen webhook-Mechanismus, um Änderungsbenachrichtigungen an Clients zu übermitteln. Ein Client ist ein Webdienst, der seine eigene URL für den Empfang von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um Ihren Status bei Änderungen zu aktualisieren. Weitere Informationen, einschließlich des Abonnierens und behandeln eingehender Benachrichtigungen, finden Sie unter Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1d7a3d868ffc640f7659623942ac102575fb94fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151492"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Verwenden der Microsoft Graph-API zum Abrufen von Änderungsbenachrichtigungen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Microsoft Graph-REST-API verwendet einen webhook-Mechanismus, um Änderungsbenachrichtigungen an Clients zu übermitteln. Ein Client ist ein Webdienst, der seine eigene URL für den Empfang von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um Ihren Status bei Änderungen zu aktualisieren. Weitere Informationen, einschließlich des Abonnierens und behandeln eingehender Benachrichtigungen, finden Sie unter [Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten](/graph/webhooks).

Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

- Outlook- [Nachricht][]
- Outlook- [Ereignis][]
- Persönlicher Outlook- [Kontakt][]
- [user][]
- [Gruppe][]
- Office 365-Gruppen [Unterhaltung][]
- Inhalt innerhalb der Hierarchie eines _beliebigen Ordners_ [DriveItem][] auf persönliche OneDrive eines Benutzers
- Inhalt in der Hierarchie des _Stammordners_ [driveItem][] auf OneDrive for Business
- Sicherheits [Warnung][]

## <a name="permissions"></a>Berechtigungen

In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.

| Berechtigungstyp                        | Unterstützte Ressourcentypen                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegiert – Geschäfts-, Schul- oder Unikonto     | [Warnung][], [Kontakt][], unter [Haltung][], [driveItem][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][]|
| Delegiert – persönliches Microsoft-Konto | [Kontakt][], [driveItem][], [Ereignis][], [Nachricht][]                                        |
| Anwendung                            | [Alert][], [Contact][], [driveItem][], [Ereignis][], [Gruppe][], [Nachricht][], [Benutzer][]|

## <a name="see-also"></a>Siehe auch

- [Abonnementressourcentyp](subscription.md)
- [Listen Abonnements](../api/subscription-list.md)
- [Abonnement abrufen](../api/subscription-get.md)
- [Abonnement erstellen](../api/subscription-post-subscriptions.md)
- [Update subscription](../api/subscription-update.md)
- [Delete subscription](../api/subscription-delete.md)

[Kontakt]: ./contact.md
[Unterhaltung]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[Warnung]: ./alert.md
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
