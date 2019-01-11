---
title: Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern
description: Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Einzelheiten, einschließlich das Abonnieren und behandeln eingehende Benachrichtigungen Set finden Sie unter Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten.
localization_priority: Normal
ms.openlocfilehash: 9b1907d37115e21b41a9e957de9b7ae0a32fd311
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816471"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Informationen zum Abonnieren und behandeln eingehende Benachrichtigungen finden Sie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks), einschließlich.

Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

- Nachrichten
- Ereignisse
- Kontakte
- Benutzer
- Gruppen
- Gruppenunterhaltungen
- OneDrive, einschließlich SharePoint-Websites zugeordneten Laufwerke freigegebenen Inhalt
- Persönliche OneDrive-Ordner von Benutzern
- Sicherheitshinweise

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
[Benutzer]: ./user.md
[Benachrichtigung]: ./alert.md
