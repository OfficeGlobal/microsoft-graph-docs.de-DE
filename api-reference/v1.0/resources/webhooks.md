---
title: Verwenden der Microsoft Graph-API, um Änderungsbenachrichtigungen zu erhalten
description: Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Änderungsbenachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren. Weitere Informationen, einschließlich der Vorgehensweise zum Abonnieren und Behandeln eingehender Benachrichtigungen, finden Sie unter "Einrichten von Benachrichtigungen für Änderungen an Benutzerdaten".
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 60def6f31ac13ad5417ad3d00e48e700550f6efe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159374"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Verwenden der Microsoft Graph-API, um Änderungsbenachrichtigungen zu erhalten

Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Änderungsbenachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren. Weitere Informationen, einschließlich der Vorgehensweise zum Abonnieren und Behandeln eingehender Benachrichtigungen, finden Sie unter [Einrichten von Benachrichtigungen für Änderungen an Benutzerdaten](/graph/webhooks).

Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

- Outlook-[Nachricht][]
- Outlook-[Ereignis][]
- Persönlicher Outlook-[Kontakt][]
- [Benutzer][]
- [Gruppe][]
- Office 365-[Gruppenunterhaltung][]
- Inhalt in der Hierarchie des [driveItem][]-Objekts eines _beliebigen Ordners_ auf dem persönlichen OneDrive eines Benutzers
- Inhalt in der Hierarchie des [driveItem][]-Objekts eines _Stammordners_ auf OneDrive for Business
- [Sicherheitswarnung][]

## <a name="permissions"></a>Berechtigungen

In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription-post-subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.

| Berechtigungstyp                        | Unterstützte Ressourcentypen                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegiert – Geschäfts-, Schul- oder Unikonto     | [alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]|
| Delegiert – persönliches Microsoft-Konto | [contact][], [driveItem][], [event][], [message][]                                        |
| Anwendung                            | [alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]|


## <a name="see-also"></a>Siehe auch

- [Abonnementressourcentyp](./subscription.md)
- [Abonnements auflisten](../api/subscription-list.md)
- [Abonnement abrufen](../api/subscription-get.md)
- [Abonnement erstellen](../api/subscription-post-subscriptions.md)
- [Abonnement aktualisieren](../api/subscription-update.md)
- [Abonnement löschen](../api/subscription-delete.md)

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
