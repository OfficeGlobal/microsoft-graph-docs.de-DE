---
title: Arbeiten mit Education-APIs in Microsoft Graph
description: Office 365-Ressourcen und Daten mit der relevante Informationen für Bildungseinrichtungen Szenarien, einschließlich Schulen, Studenten, Lehrer, Klassen, Registrierung und Zuordnungen der Education-APIs in Microsoft Graph zu verbessern. Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516931"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Arbeiten mit Education-APIs in Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Office 365-Ressourcen und Daten mit der relevante Informationen für Bildungseinrichtungen Szenarien, einschließlich Schulen, Studenten, Lehrer, Klassen, Registrierung und Zuordnungen der Education-APIs in Microsoft Graph zu verbessern. Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.

Die Education umfassen APIs Rostering und Zuordnungen Ressourcen, die Sie für die Interaktion mit den Rostering und Zuweisen von Diensten in Microsoft-Teams verwenden können. Diese Ressourcen können Sie eine Schule Teilnehmerliste verwalten und Automatisierung von Hausaufgaben.

## <a name="authorization"></a>Autorisierung

Damit die Education-APIs in Microsoft Graph aufgerufen werden können, muss Ihre App ein Zugriffstoken erwerben. Weitere Informationen zu Zugriffstoken finden Sie unter [Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Zudem muss Ihre App über die entsprechenden Berechtigungen verfügen. Weitere Informationen finden Sie unter [Education-Berechtigungen](/graph/permissions-reference#education-permissions). 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>App-Berechtigungen zum Aktivieren der Zustimmung von Schul-IT-Administratoren 

Um Apps bereitzustellen, die in Education-APIs in Microsoft Graph integriert sind, müssen Schul-IT-Administratoren zunächst ihre Zustimmung für die von der App angeforderten Berechtigungen erteilen. Diese Zustimmung muss nur einmal erteilt werden, sofern sich die Berechtigungen nicht ändern. Nachdem der Administrator seine Zustimmung erteilt hat, wird die App für alle Benutzer im Mandanten bereitgestellt.

Verwenden Sie den folgenden REST-Aufruf, um ein Dialogfeld für die Zustimmung auszulösen.

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|Parameter|Beschreibung|
|:--------|:----------|
|Mandant|Mandanten-ID der Schule. Verwenden Sie die vollständige-ID, die „onmicrosoft.com“ enthält.|
|clientId|Client-ID der App.|
|redirectUrl|App-Umleitungs-URL.|


## <a name="rostering"></a>Listenerstellung

Mit Listenerstellungs-APIs können Sie Daten von einem Office 365-Mandanten der Schule extrahieren, der mit [Microsoft School Data Sync](https://sds.microsoft.com/) bereitgestellt wurde. Diese APIs bieten Zugriff auf Informationen zu Schulen, Abschnitten, Lehrern, Schülern, Studenten und Listen. Die APIs unterstützen sowohl Szenarien vom Typ „Nur App“ (Synchronisierung) als auch vom Typ „App und Benutzer“ (interaktiv). APIs, die interaktive Szenarien unterstützen, erzwingen auf Grundlage der Benutzerrolle, die die API aufruft, regionsspezifische RBAC-Richtlinien. Dies ermöglicht eine konsistente API und eine minimale Richtlinienoberfläche, unabhängig von der Verwaltungskonfiguration innerhalb der Mandanten. Die APIs bieten darüber hinaus auch bildungsspezifische Berechtigungen, um sicherzustellen, dass der richtige Benutzer auf die Daten zugreifen kann.

Mithilfe von Listenerstellungs-APIs erhält der App-Benutzer Antworten auf die folgenden Fragen:

- Wer bin ich?
- An welchen Kursen nehme ich teil bzw. welche Kurse unterrichte ich?
- Was muss ich wann tun?

Die Listenerstellungs-APIs bieten die folgenden zentralen Ressourcen:

- [educationSchool](educationschool.md): Schule.
- [educationClass](educationclass.md): Kurs in einer Schule.
- [educationTerm](educationterm.md): Ein festgelegter Teil des akademischen Jahres.
- [educationTeacher](educationteacher.md): Ein Benutzer mit der primären Rolle „Lehrer“.
- [educationStudent](educationstudent.md): Ein Benutzer mit der primären Rolle „Schüler/Student“.

Die Listenerstellungs-APIs unterstützen die folgenden Szenarien:

- [Auflisten aller Schulen](../api/educationroot-list-schools.md) 
- [Auflisten von Schulen, in denen ein Kurs unterrichtet wird](../api/educationclass-list-schools.md)
- [Auflisten von Schulen für einen Benutzer](../api/educationuser-list-schools.md)
- [Abrufen aller Kurse](../api/educationroot_list_classes.md )
- [Abrufen von Kursen einer Schule](../api/educationschool-list-classes.md)
- [Auflisten von Kursen für einen Benutzer](../api/educationuser-list-classes.md)
- [Hinzufügen von Kursen zu einer Schule](../api/educationschool-post-classes.md)
- [Abrufen von Schülern/Studenten und Lehrern für einen Kurs](../api/educationclass-list-members.md)
- [Hinzufügen von Mitgliedern zu einem Kurs](../api/educationclass-post-members.md) 
- [Auflisten von Lehrern für einen Kurs](../api/educationclass-list-teachers.md)
- [Abrufen von Benutzern in einer Schule](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Zuordnungen 

Die Education Assignment-bezogene APIs können Sie um Zuordnungen in Microsoft-Teams, zu integrieren. Microsoft-Teams in Office 365 für Bildungseinrichtungen basiert auf der gleichen Education-APIs und bietet einen Anwendungsfall für die Arbeit mit den APIs. Ihre app kann diese APIs Interaktion mit Zuordnungen im gesamten Lebenszyklus Zuordnung verwenden. 

Die Zuordnung APIs bieten die folgenden wichtigen Ressourcen:

- [EducationAssignment](educationassignment.md) - Core-Objekts der Zuordnungen API. Stellt einen Vorgang oder eine Arbeitsschritt Mitglied Student oder ein Team in einer Klasse als Teil ihrer Studie zugewiesen.
- [EducationSubmission](educationsubmission.md) – stellt die Ressourcen, die eine einzelne (oder Gruppe) für eine Zuordnung und die zugehörigen Note und Feedback für diese Aufgabe sendet.
- [EducationResource](educationresource.md) - stellt also das Learning-Objekt zugewiesen wird, oder übermittelt. Ein **EducationResource** ist ein **EducationAssignment** und/oder ein **EducationSubmission**zugeordnet.

Die Zuordnung APIs unterstützen die folgenden Szenarien:

- [Erstellen der Zuordnung](../api/educationclass-post-assignments.md)
- [Zuordnung veröffentlichen](../api/educationassignment-publish.md)
- [Erstellen der Zuordnung Ressource](../api/educationassignment-post-resources.md)
- [Erstellen Sie zum Absenden-Ressource](../api/educationsubmission-post-resources.md)
- [Aufgabe abgeben](../api/educationsubmission-submit.md) 
- [Zuordnung unsubmit](../api/educationsubmission-unsubmit.md)   
- [Klassen und Feedback zur Student zurückzukehren.](../api/educationsubmission-return.md) 
- [Abrufen von Zuordnungsdetails](../api/educationuser-list-assignments.md)

Es folgen einige allgemeine Verwendungsszenarien für die Zuordnung-bezogene Bildungseinrichtungen APIs.

|Anwendungsfall|Beschreibung|Siehe auch|
|:-------|:----------|:-------|
|Erstellen von Aufgaben|Ein externes System kann eine Zuordnung für die Klasse erstellt und die Zuordnung Ressourcen zuordnen.|[Erstellen der Zuordnung](../api/educationassignment-post-resources.md)|
|Lesen Sie die Informationen zur Zuordnung|Eine Anwendung Analytics erhalten Informationen zu Aufgaben und Student Übermittlungen, einschließlich Datums- und Klassen.|[Abrufen der Zuordnung](../api/educationassignment-get.md)|
|Nachverfolgen von Student Übermittlungen|Ihre app kann ein Dashboard Lehrer bereitstellen, das zeigt, wie viele eingereichten Studenten bewertet werden müssen.|[Übermittlung Ressource](educationsubmission.md)|

## <a name="school-data-sync-management"></a>Schule Sync-Verwaltung

[Schule Daten Sync](https://sds.microsoft.com/) hilft importieren und Synchronisieren von Daten aus Student Informationssysteme Teilnehmerliste einer mit Azure Active Directory (AD Azure) und Office 365 automatisieren. Sync-datenverwaltung Schule APIs können in Microsoft Graph Sie aus einer CSV-Datei oder einen unterstützten SIS API-Connector-Synchronisierung einrichten.

Die Schuldaten synchronisieren Management APIs unterstützt die folgenden Szenarien:

- [Liste Synchronisierungsprofile](../api/educationsynchronizationprofile-list.md)
- [Synchronisierung Profil abrufen](../api/educationsynchronizationprofile-get.md)
- [Erstellen Sie Synchronisierung Profil](../api/educationsynchronizationprofile-post.md)
- [Synchronisierung Profil löschen](../api/educationsynchronizationprofile-delete.md)
- [Eine laufende Synchronisierung anhalten](../api/educationsynchronizationprofile-pause.md)
- [Fortsetzen einer angehaltenen sync](../api/educationsynchronizationprofile-resume.md)
- [Zurücksetzen einer Synchronisierung](../api/educationsynchronizationprofile-reset.md)
- [Synchronisierung für Uploaddateien starten](../api/educationsynchronizationprofile-start.md) 
- [Abrufen einer Upload-URL](../api/educationsynchronizationprofile-uploadurl.md)
- [Abrufen des Status der Synchronisierung](../api/educationsynchronizationprofilestatus-get.md)
- [Abrufen von Synchronisierungsfehler](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>Nächste Schritte
Verwenden Sie das Microsoft Graph Education APIs Education-Lösungen zu erstellen, der Hausaufgaben und Schule konferenzlisten zugreifen. So erhalten Sie weitere Informationen:

- Erfahren Sie, welche Ressourcen und Methoden für Ihr Szenario am besten geeignet sind.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
