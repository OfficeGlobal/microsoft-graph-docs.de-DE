# <a name="share-outlook-message-folders-between-users"></a>Freigeben von Outlook-Nachrichtenordnern zwischen Benutzern

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

In Outlook können Kunden Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner oder das gesamte Postfach gewähren. Dies wird in Outlook auch als „Delegierung“ bezeichnet.

Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst.

Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.

## <a name="get-a-message-in-the-shared-folder"></a>Abrufen einer Nachricht im freigegebenen Ordner

Sie können eine bestimmte Nachricht in Garths Posteingang abrufen:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und die [message](../api-reference/v1.0/resources/message.md)-Instanz mit der ID `{id}` aus Garths Posteingang.

## <a name="get-all-messages-in-the-shared-folder"></a>Abrufen aller Nachrichten im freigegebenen Ordner

So rufen Sie alle Nachrichten in Garths Posteingang ab:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine Sammlung der [message](../api-reference/v1.0/resources/message.md)-Instanzen in Garths Posteingang.

## <a name="get-the-shared-folder"></a>Abrufen des freigegebenen Ordners

Rufen Sie den Ordner (Posteingang) ab, den Garth für John freigegeben hat.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine [mailFolder](../api-reference/v1.0/resources/mailfolder.md)-Instanz, die den Ordner „Posteingang“ von Garth darstellt.

Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Posteingang delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.

Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben. 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Gründe für die Integration in Outlook-Mail](outlook-mail-concept-overview.md)
- [Verwenden der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) für diese in Microsoft Graph v1.0.