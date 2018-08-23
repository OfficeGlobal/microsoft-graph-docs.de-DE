# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Verwenden der Microsoft Graph-API zum Erhalten von Änderungsbenachrichtigungen

Die Microsoft Graph-REST-API sendet mithilfe eines Webhook-Mechanismuses Benachrichtigungen an Clients. Ein Client ist ein Web-Service, der seine eigene URL konfiguriert, um Benachrichtigungen zu erhalten. Client-Apps nutzen Benachrichtigungen, um bei Änderung ihren Status zu aktualisieren. Weitere Informationen zum Abonnieren und Verwalten von eingehenden Benachrichtigungen finden Sie unter [Benachrichtigungen für Änderungen bei Benutzerdaten festlegen](../../../concepts/webhooks.md).

Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

- Nachrichten
- Ereignisse
- Kontakte
- Benutzer
- Gruppen
- Gruppenunterhaltungen
- Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke
- Persönliche OneDrive-Order von Benutzern

## <a name="permissions"></a>Berechtigungen

In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api/subscription_post_subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann.

| Berechtigungstyp                        | Unterstützte Ressourcentypen in v1.0                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| Delegiert – Geschäfts-, Schul- oder Unikonto     | [Kontakt][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Nachricht][] |
| Delegiert – persönliches Microsoft-Konto | Keine                                                             |
| Anwendung                            | [Kontakt][], [Unterhaltung][], [Ereignis][], [Nachricht][]            |

## <a name="see-also"></a>Siehe auch

- [Abonnementressourcentyp](./subscription.md)
- [Abonnement abrufen](../api/subscription_get.md)
- [Abonnement erstellen](../api/subscription_post_subscriptions.md)
- [Abonnement aktualisieren](../api/subscription_update.md)
- [Abonnement löschen](../api/subscription_delete.md)

[Kontakt]: ./contact.md
[Unterhaltung]: ./conversation.md
[Laufwerk]: ./drive.md
[Ereignis]: ./event.md
[Nachricht]: ./message.md
