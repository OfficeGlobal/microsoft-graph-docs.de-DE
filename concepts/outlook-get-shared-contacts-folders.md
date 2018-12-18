---
title: Abrufen von Outlook-Kontakten in einem freigegebenen Ordner
description: " es gibt außerdem "
author: angelgolfer-ms
ms.openlocfilehash: a3dd8cff5cac88d3ef273b63f40bc8af87910aa1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315176"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>Abrufen von Outlook-Kontakten in einem freigegebenen Ordner

In Outlook können Kunden Ordner für andere freigeben und den Zugriff zum Lesen, Erstellen oder Ändern auf einzelne Kontaktordner erteilen. In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, im Auftrag des Kunden zu handeln und auf bestimmte Ordner oder das gesamte Kundenpostfach zugreifen. Dies wird in Outlook auch als "Delegierung" bezeichnet.

Programmgesteuert unterstützt Microsoft Graph das Abrufen von Kontakten in Kontaktordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst. Die Unterstützung gilt auch für Ordner in einem delegierten Postfach.

Beispielsweise hat Adrian für John einen benutzerdefinierten Kontaktordner freigegeben und John Lesezugriff erteilt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Contacts.Read.Shared oder Contacts.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Adrians benutzerdefinierten Kontaktordner und auf die Kontakte in diesem Ordner zugreifen, wie nachstehend beschrieben.

## <a name="get-a-contact-in-the-shared-folder"></a>Abrufen eines Kontakts im freigegebenen Ordner

Sie können einen bestimmten Kontakt im benutzerdefinierten Kontaktordner abrufen, den Adrian für John freigegeben hat:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und die [contact](/graph/api/resources/contact?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Adrians freigegebenem Kontaktordner.

## <a name="get-all-contacts-in-the-shared-folder"></a>Abrufen aller Kontakte im freigegebenen Ordner

Abrufen aller Kontakte in Adrians freigegebenem Kontaktordner:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine Sammlung der [contact](/graph/api/resources/contact?view=graph-rest-1.0)-Instanzen in Adrians freigegebenem Kontaktordner.

## <a name="get-the-shared-folder"></a>Abrufen des freigegebenen Ordners

Abrufen des Kontaktordners, den Adrian für John freigegeben hat.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)-Instanz, die Adrians freigegebenen Kontaktordner darstellt.

Die gleichen GET-Funktionen würden ebenfalls gelten, wenn Adrian sein gesamtes Postfach an John delegiert hätte.

Wenn Adrian weder den Kontaktordner für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe von Adrians Benutzer-ID oder seines Benutzerprinzipalnamens bei diesen GET-Vorgängen ein Fehler zurückgegeben. 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Warum persönliche Kontakte in Outlook integrieren?](outlook-contacts-concept-overview.md)
- Die [Kontakte-API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0