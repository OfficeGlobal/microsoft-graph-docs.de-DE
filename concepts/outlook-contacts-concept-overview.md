---
title: Übersicht über die Persönliche Kontakte-API
description: Über Outlook-Kontakte können Sie die Daten von persönlichen Kontakten speichern; sie sind Teil des Outlook-Messaging-Hubs in Office 365. Über Outlook können Sie E-Mails verwalten, Besprechungen planen, Informationen zu Benutzern in einer Organisation suchen, Onlineunterhaltungen initiieren, Dateien freigeben und in Gruppen zusammenarbeiten.
ms.openlocfilehash: 0e8967fbb89b2d39e002826e9eb3f7f792c37a11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092150"
---
# <a name="outlook-personal-contacts-api-overview"></a>Übersicht über die Persönliche Kontakte-API

Über Outlook-Kontakte können Sie die Daten von persönlichen Kontakten speichern; sie sind Teil des Outlook-Messaging-Hubs in Office 365. Über Outlook können Sie E-Mails verwalten, Besprechungen planen, Informationen zu Benutzern in einer Organisation suchen, Onlineunterhaltungen initiieren, Dateien freigeben und in Gruppen zusammenarbeiten.

## <a name="why-integrate-with-outlook-personal-contacts"></a>Warum persönliche Kontakte in Outlook integrieren?

### <a name="complement-messaging-and-calendaring-scenarios-for-hundreds-of-millions-of-customers"></a>Ergänzung von Messaging- und Kalenderszenarien für hunderte Millionen von Kunden

Hunderte Millionen Kunden und mehrere zehn Millionen Organisationskunden nutzen Outlook als E-Mail-Client. Kontakte bieten eine ergänzende Funktion für Messaging- und Kalenderfunktionen, indem Kunden eine praktischen, integrierten Speicher von Kontaktdaten innerhalb von Outlook pflegen können. Die Nutzung der vielfältigen Funktionen von [E-Mails](outlook-mail-concept-overview.md) oder des [Kalenders](outlook-calendar-concept-overview.md) bedeutet für Entwickler umfassendere Szenarien mit den Kontaktdaten von Benutzern.


### <a name="automate-contact-organization"></a>Automatisieren der Kontaktorganisation

Mit der Kontakte-API können Sie Ihre Kunden organisieren, und zwar in sehr ähnlicher Weise wie die Kunden dies selbst über Outlook tun:

- Ähnlich wie bei der Kundenoberfläche können Sie [contact](/graph/api/resources/contact?view=graph-rest-1.0)-Instanzen erstellen und diese [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)-Objekten zuordnen.
- Mit der Kontakte-API können Sie Kategorien, Kontakte, Ereignisse, Nachrichten, Aufgaben und Gruppenbeiträge konsistent zuweisen, um die Organisation und Ermittlung zu verbessern. Darüber hinaus können Sie [eine Masterliste von Kategorien eines Benutzers definieren](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), was weitere Szenarien eröffnen kann.
- Sie können für einen [Kontakt](/graph/api/resources/contact?view=graph-rest-1.0) eine Kennzeichnung zur Nachverfolgung festlegen. (Das Kennzeichnen befindet sich in Microsoft Graph derzeit [in der Vorschau](versioning-and-support.md#beta-version).)


### <a name="share-contact-information"></a>Freigeben von Kontaktinformationen

Mit der Kontakte-API können Sie Kontaktelemente des angemeldeten Benutzers oder von Benutzern, die ihre Kontakte für den angemeldeten Benutzer freigegeben oder an ihn delegiert haben, abrufen. Wenn Garth beispielsweise einen Kontaktordner für John freigegeben hat oder wenn Garth John Zugriff erteilt hat, so würden Sie über [delegierte Berechtigungen](permissions-reference.md#delegated-permissions-application-permissions-and-effective-permissions) von John Lesezugriff auf den freigegebenen Kalender und auch auf die Inhalte erhalten.


### <a name="leverage-people-api-in-microsoft-graph-to-make-better-use-of-all-people-data"></a>Nutzen der Personen-API in Microsoft Graph zur besseren Ausnutzung aller Personendaten

Sie können die normalen CRUD-Vorgänge für einen Outlook-[Kontakt](/graph/api/resources/contact?view=graph-rest-1.0) zum Erstellen und Verwalten von Kontakten verwenden. Im Rahmen von Microsoft Graph können Sie auch die [Personen-API](people-example.md) verwenden, die sich die Outlook-Kontakte eines Benutzers sowie die sozialen Netzwerke, das Unternehmensverzeichnis und Personen aus kürzlichen Kommunikationen ansieht und Informationen zu Personen aus all diesen Quellen zurückgibt, die für den Benutzer am wichtigsten sind. Nutzen Sie diese zusätzliche Intelligenz in Personenauswahlszenarien.


### <a name="take-advantage-of-other-shared-features-and-conveniences-in-microsoft-graph"></a>Nutzen der Vorteile anderer freigegebener Features und Vorteile von Microsoft Graph

- Die **contact**-Entität unterstützt ein Kontaktfoto, das als dieselbe [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-1.0)-Entität wie ein in Exchange Online oder Azure Active Directory gespeichertes Benutzerfoto implementiert wird. Dadurch wird der Aufwand des Konvertierens von Kontakten und Benutzerprofilfotos reduziert.
- Sie können den lokalen App-Speicher synchronisieren, indem Sie [Änderungsbenachrichtigungen](/graph/api/resources/webhooks?view=graph-rest-1.0) und [Nachverfolgungsänderungen](delta-query-overview.md) an Kontakten und Kontaktordnern abonnieren.
- Sie können den App-Speicher in einer Kontaktinstanz als [offene Erweiterung](extensibility-overview.md#open-extensions) erweitern oder stark typisierte benutzerdefinierte Daten als [Schemaerweiterung](extensibility-overview.md#schema-extensions) hinzufügen.

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [Outlook-Kontakte-API in Microsoft Graph v1.0](/graph/api/resources/contact?view=graph-rest-1.0)
- [Outlook-Kontakte-API in Microsoft Graph, Betaversion](/graph/api/resources/contact?view=graph-rest-beta)

## <a name="next-steps"></a>Nächste Schritte

- Wählen Sie Beispielabfragen für Kontakte in [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fcontacts&version=v1.0) aus. Wählen Sie in der Spalte links **Mehr Beispiele anzeigen** aus. Aktivieren Sie **Persönliche Kontakte** über das Menü.
- Informieren Sie sich über folgende Themen:
  - [Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen](outlook-immutable-id.md)
  - [Abrufen von freigegebenen Kontakten](outlook-get-shared-contacts-folders.md)
- Sehen Sie sich die Referenz zur Outlook-[Kontakte-API](/graph/api/resources/contact?view=graph-rest-1.0) an.
