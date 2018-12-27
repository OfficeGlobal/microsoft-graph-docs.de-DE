---
title: Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner
description: In Outlook können Kunden E-Mail-Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner gewähren. In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, um im Auftrag des Kunden zu handeln.
author: angelgolfer-ms
ms.openlocfilehash: cdb2228c64647497674402825577942323c3d2ff
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413176"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner

In Outlook können Kunden E-Mail-Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner gewähren. In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, im Auftrag des Kunden zu handeln und auf bestimmte E-Mail-Ordner oder das gesamte Kundenpostfach zugreifen. Dies wird in Outlook auch als „Delegierung“ bezeichnet.

Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst. Die Unterstützung gilt auch für Ordner, die delegiert wurden.

Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.

> **Hinweis** Mithilfe der Freigabeberechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) können Sie Ereignisse in einem freigegebenen oder delegierten Ordner lesen oder schreiben. [Das Abonnieren von Änderungsbenachrichtigungen](webhooks.md) wird für Elemente in solchen Ordnern nicht unterstützt. Verwenden Sie zum Einrichten von Änderungsbenachrichtigungsabonnements für Nachrichten in einem freigegebenen, delegierten oder einem Postfachordner eines anderen Benutzers im Mandanten die Berechtigung „Mail.Read“.

## <a name="get-a-message-in-the-shared-folder"></a>Abrufen einer Nachricht im freigegebenen Ordner

Sie können eine bestimmte Nachricht in Garths Posteingang abrufen:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und die [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Garths Posteingang.

## <a name="get-all-messages-in-the-shared-folder"></a>Abrufen aller Nachrichten im freigegebenen Ordner

So rufen Sie alle Nachrichten in Garths Posteingang ab:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine Sammlung der [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanzen in Garths Posteingang.

## <a name="get-the-shared-folder"></a>Abrufen des freigegebenen Ordners

Rufen Sie den Ordner (Posteingang) ab, den Garth für John freigegeben hat.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)-Instanz, die den Ordner „Posteingang“ von Garth darstellt.

Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Posteingang delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.

Wenn Garth weder seinen Posteingang für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben. 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Gründe für die Integration in Outlook-Mail](outlook-mail-concept-overview.md)
- [Verwenden der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) für diese in Microsoft Graph v1.0.