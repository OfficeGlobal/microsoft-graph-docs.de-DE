---
title: Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner
description: Diese Themen haben auch ähnliche Abschnitte – Ereignisse auflisten, Ereignis abrufen, Kontakte auflisten, Kontakt abrufen, Kontaktordner abrufen.
ms.openlocfilehash: d9e04527879cb32f14dc8d74a814a54150c5b2d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092250"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

In Outlook können Kunden E-Mail-Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner gewähren. In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, im Auftrag des Kunden zu handeln und auf bestimmte E-Mail-Ordner oder das gesamte Kundenpostfach zugreifen. Dies wird in Outlook auch als „Delegierung“ bezeichnet.

Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst. Die Unterstützung gilt auch für Ordner, die delegiert wurden.

Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.

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