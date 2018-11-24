# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Verwenden der Microsoft Graph-API zum Abrufen Benachrichtigungen ändern

Die Microsoft Graph-REST-API verwendet einen Webhook Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der den eigenen URL Erhalt von Benachrichtigungen konfiguriert. Client-apps verwenden Benachrichtigungen, um deren Status nach Änderungen zu aktualisieren. Weitere Informationen zum Abonnieren und behandeln eingehende Benachrichtigungen finden Sie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](../../../concepts/webhooks.md), einschließlich.

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

In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription_post_subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.

| Berechtigungstyp                        | Unterstützte Ressourcentypen in v1.0                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| Delegiert – Geschäfts-, Schul- oder Unikonto     | [wenden Sie sich an][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Nachricht][], [Benachrichtigung][] |
| Delegiert – persönliches Microsoft-Konto | Keine                                                             |
| Anwendung                            | [wenden Sie sich an][], [Unterhaltung][], [Ereignis][], [Nachricht][], [Benachrichtigung][]           |

## <a name="see-also"></a>Siehe auch

- [Abonnementressourcentyp](./subscription.md)
- [Abonnement abrufen](../api/subscription_get.md)
- [Abonnement erstellen](../api/subscription_post_subscriptions.md)
- [Update subscription](../api/subscription_update.md)
- [Delete subscription](../api/subscription_delete.md)

[Kontakt]: ./contact.md
[Unterhaltung]: ./conversation.md
[Laufwerk]: ./drive.md
[Ereignis]: ./event.md
[Nachricht]: ./message.md
[Benachrichtigung]: ./alert.md