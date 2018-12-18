---
title: Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender
description: In Outlook können Kunden einen Kalender mit anderen Benutzern teilen und sie Ereignisse in diesem Kalender anzeigen oder ändern lassen. Kunden können außerdem eine Stellvertretung für das Handeln in ihrem Auftrag erteilen, um Besprechungsanfragen zu empfangen oder zu beantworten oder um Elemente im Kalender zu erstellen oder zu ändern.
author: angelgolfer-ms
ms.openlocfilehash: 8ceb6a49b971c5ad01f27b53c0f3cd3cf047865d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346564"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender

In Outlook können Kunden einen Kalender mit anderen Benutzern teilen und sie Ereignisse in diesem Kalender anzeigen oder ändern lassen. Kunden können außerdem eine Stellvertretung für das Handeln in ihrem Auftrag erteilen, um Besprechungsanfragen zu empfangen oder zu beantworten oder um Elemente im Kalender zu erstellen oder zu ändern.

Programmgesteuert unterstützt Microsoft Graph das Abrufen von Ereignissen in Kalendern, die von anderen Benutzern geteilt wurden, sowie das Abrufen der Kalender selbst. Die Unterstützung gilt auch für Kalender, die delegiert wurden.

Beispielsweise hat Adrian für John seinen Standardkalender freigegeben und John Lesezugriff erteilt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Calendars.Read.Shared oder Calendars.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Adrians Standardkalender und auf die Ereignisse in diesem Kalender zugreifen, wie nachstehend beschrieben.

## <a name="get-an-event-in-the-shared-calendar"></a>Abrufen eines Ereignisses im freigegebenen Kalender

Sie können ein bestimmtes Ereignis in Adrians freigegebenem Standardkalender abrufen:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und die [event](/graph/api/resources/event?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Adrians Posteingang.

## <a name="get-all-the-events-in-the-shared-calendar"></a>Abrufen aller Ereignisse im freigegebenen Kalender

Rufen Sie alle Ereignisse im Standardkalender ab, den Adrian mit John geteilt hat:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine Sammlung der [event](/graph/api/resources/event?view=graph-rest-1.0)-Instanzen in Adrians Standardkalender.

## <a name="get-the-shared-calendar"></a>Abrufen des freigegebenen Kalenders

Rufen Sie den Standardkalender ab, den Adrian mit John geteilt hat.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine [calendar](/graph/api/resources/calendar?view=graph-rest-1.0)-Instanz, die Adrians Standardordner darstellt.

Dieselben GET-Funktionen würden gelten, wenn Adrian an John weiteren Zugriff auf Adrians Standardkalender delegiert hätte oder wenn Adrian sein gesamtes Postfach an John delegiert hätte.

Wenn Adrian weder seinen Standardkalender für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe von Adrians Benutzer-ID oder seines Benutzerprinzipalnamens in diesen GET-Vorgängen ein Fehler zurückgegeben. 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Vorteile der Integration mit dem Outlook-Kalender](outlook-calendar-concept-overview.md)
- Die [Kalender-API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0