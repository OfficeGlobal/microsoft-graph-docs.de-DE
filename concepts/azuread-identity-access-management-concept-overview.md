---
title: Überblick über die Azure AD-Identitäts- und Zugriffsverwaltungs-API
description: 'Azure Active Directory (Azure AD) unterstützt die Zentralisierung der Identitäts- und Zugriffsvererwaltung (Identity and Access Management, IAM), um den sicheren und produktiven Zugriff zwischen Apps, Geräten, Diensten und der Infrastruktur zu gewährleisten. Unternehmen können mit Azure AD Identitäten verwalten und den Zugriff in lokalen, Hybrid- und Cloudumgebungen steuern.  '
ms.openlocfilehash: f933e47f890f228865968d47040fdb1316607692
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156047"
---
# <a name="azure-ad-identity-and-access-management-api-overview"></a>Überblick über die Azure AD-Identitäts- und Zugriffsverwaltungs-API

Azure Active Directory (Azure AD) unterstützt die Zentralisierung der Identitäts- und Zugriffsvererwaltung (Identity and Access Management, IAM), um den sicheren und produktiven Zugriff zwischen Apps, Geräten, Diensten und der Infrastruktur zu gewährleisten. Unternehmen können mit Azure AD Identitäten verwalten und den Zugriff in lokalen, Hybrid- und Cloudumgebungen steuern.  

Sie können die Azure AD-REST-APIs in Microsoft Graph zum Erstellen von eindeutigen Workflows zwischen Azure AD-[Ressourcen](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0) und Diensten von Drittanbietern verwenden.

## <a name="why-use-the-azure-ad-apis"></a>Vorteile für die Verwendung der Azure AD-APIs

Mehr als 15 Millionen Organisationen verwenden Azure AD im Rahmen ihrer Abonnements von Microsoft-Clouddiensten wie Office 365, Microsoft Azure, Enterprise Mobility Suite oder Microsoft 365.  

Enterprise-Entwickler verwenden Microsoft Graph zur Integration von Azure AD-Identitätsmanagement und anderen Diensten, um Verwaltungsworkflows wie z. B. das Mitarbeiter-Onboarding (und Beendigung des Arbeitsverhältnisses), die Pflege von Profilen, die Lizenzbereitstellung und vieles mehr zu automatisieren.

Microsoft Graph und Azure AD unterstützen viele Enterprise-Entwickler dabei, vorhandene Anwendungen für die Cloud vorzubereiten und darin zu verschieben, um so die digitale Transformation eines Unternehmens zu beschleunigen. Sie können die Vorteile der Azure AD-Funktionen nutzen, um Anwendungen Mechanismen für die Zugriffssteuerung hinzuzufügen. So können Sie zum Beispiel die Gruppenmitgliedschaft eines Benutzers, die Directory-Rolle oder die Mitgliedschaft bei einer administrativen Gruppe überprüfen.

Sie können Microsoft Graph und Azure AD als Möglichkeit nutzen, schnell und einfach mehr als 15 Millionen Organisationen zu erreichen, einschließlich 90 % der Fortune 500-Unternehmen, die bereits Azure AD-Dienste verwenden. Integrierte Anwendungen ermöglichen nahtlose Oberflächen für die Anmeldung und können mit vorhandenen Unternehmensdaten angepasste Oberflächen erstellen.  

Sie können die Azure AD-APIs in Microsoft Graph verwenden, um das Profil eines Benutzers abzufragen, andere Benutzer zu suchen, Geschäftsbeziehungen zu verwalten, Aufgaben nachzuverfolgen oder eigene Lösungen zu erstellen, die vorhandene Unternehmensdaten einbeziehen. Diese APIs bieten eine solide Grundlage, um benutzerdefinierte Geschäftsanwendungen nahtlos in vorhandene digitale Dienste eines Unternehmens zu integrieren.

### <a name="access-users-and-groups"></a>Zugreifen auf Benutzer und Gruppen

Mit den Azure AD-APIs in Microsoft Graph haben Sie die folgenden Möglichkeiten:

- Suchen Sie nach und verwalten Sie [Benutzerprofilinformationen](/graph/api/resources/user?view=graph-rest-1.0) zu Benutzern in Ihrer Organisation, wie z. B. Name, Foto, E-Mail-Adresse, Position, Bürostandort und vieles mehr.
- Erstellen Sie [Gruppen](/graph/api/resources/groups-overview?view=graph-rest-1.0) für Projekte und Teams in Ihrer Organisation. Fügen Sie der Gruppe Mitglieder hinzu, oder entfernen Sie Mitglieder aus der Gruppe, um den Zugriff auf Ressourcen zu steuern. (Dynamische Gruppen können automatisch basierend auf Benutzereigenschaftswerten die Mitgliedschaft ändern.)
- Um den Zugriff zu steuern, können Sie nach einer [transitiven Mitgliedschaft](/graph/api/user-checkmembergroups?view=graph-rest-1.0) in einer Liste der Gruppen suchen, oder Sie können alle Ressourcen eines bestimmten Typs (z. B. Benutzer oder Gruppe) aus einer Liste mit [generischen Ressource-IDs](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) abrufen.

### <a name="manage-directory-roles"></a>Verwalten von Directory-Rollen

Können Sie Benutzer vordefinierten administrativen Azure AD-[Directory-Rollen](/graph/api/resources/directoryrole?view=graph-rest-1.0) zuweisen, die Berechtigungen zum Ausführen bestimmter Aufgaben gewähren.

### <a name="manage-devices"></a>Verwalten von Geräten

[Verwalten Sie Geräte](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction), die in der Organisation registriert sind. Geräte sind für Benutzer registriert und umfassen Elemente wie Laptops, Desktops, Tablets und Mobiltelefone. Geräte werden in der Regel mithilfe des Geräteregistrierungsdiensts oder von Microsoft Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet.

### <a name="partner-tenant-management"></a>Verwaltung von Partnermandanten

Microsoft-Partnern, die Microsoft Online Services (z. B. Office 365, Microsoft Azure und CRM Online) verkaufen und verwalten, können die [Organisationsmandanten](/graph/api/resources/contract?view=graph-rest-1.0)anzeigen,die sie derzeit verwalten.

Sie können auch die [Domänen verwalten](/graph/api/resources/domain?view=graph-rest-1.0), die mit einem Mandanten verknüpft sind. Mithilfe von Domänenvorgängen können Microsoft-Partner die Domänenregistrierung für Dienste wie Office 365 automatisieren.

### <a name="tenant-management"></a>Verwaltung von Mandanten

Azure AD-APIs für die Verwaltung von Mandanten bieten Ihnen die folgenden Möglichkeiten:

- Abrufen von Informationen über eine [Organisation](/graph/api/resources/organization?view=graph-rest-1.0), z. B. die Unternehmensadresse, Kontakte für technische Fragen und Benachrichtigungen, aktive Dienstabonnements sowie die Domänen, die mit damit verknüpft sind.
- Abrufen von Informationen über die [Dienst-SKUs](/graph/api/resources/subscribedsku?view=graph-rest-1.0), die ein Unternehmen abonniert hat.
- [Einladen externer](/graph/api/resources/invitation?view=graph-rest-1.0) (Gast)Benutzer zu einer Organisation.

### <a name="monitor-identity-risks-preview"></a>Überwachen von Risiken (Preview)

Die meisten Sicherheitsverletzungen entstehen dadurch, dass Angreifer die Identität eines Benutzers stehlen. Zudem nutzen Angreifer erschreckend effektiv Sicherheitsrisiken durch Drittanbieter, Password-Spray-Angriffe und ausgeklügelte Phishingangriffe aus. Dies bedeutet, dass Sie alle Benutzerkonten vor diesen Angriffen schützen und proaktiv verhindern müssen, dass manipulierte Identitäten missbraucht werden können.

Azure Active Directory verwendet adaptive Machine Learning-Algorithmen und Heuristiken, um Anomalien zu erkennen, die auf potenziell kompromittierte Konten hinweisen. Verwenden diese Daten, Azure AD-Schutz schützt die Benutzer mit Risiko-basierte bedingte Zugriffsrichtlinien und generiert Berichte und Warnungen auf seine erkannte.

Microsoft Graph gibt heute Zugriff auf Kunden von Azure AD Premium P2 bis [Abfrageereignissen Risiko von Schutz erkannt](/graph/api/resources/identityprotection-root?view=graph-rest-beta), einschließlich des Risikoereignis Typ, Schweregrad, Datum, Uhrzeit, Ort, betroffenen Benutzer und mehr. Kunden können dann diese Ereignisse in SIEM-Systeme und Sicherheit Applikationen verwenden.

### <a name="activate-users-into-privileged-roles-preview"></a>Aktivieren von Benutzern in privilegierte Rollen (Vorschau)

Sie können sicheren Zugriff auf Ressourcen erlangen, indem Sie Administratorberechtigungen bei Bedarf aktivieren. [Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) ist ein Feature von Azure AD Premium P2.

### <a name="manage-user-access-reviews-preview"></a>Verwalten von Benutzer Zugriff Bewertungen (Preview)

Sie können Access Bewertungen von Gruppenmitgliedschaften und Zugriff auf die Anwendung konfigurieren. [Access überprüft](/graph/api/resources/accessreviews-root?view=graph-rest-beta) ist in Azure AD Premium P2 enthalten.

## <a name="api-reference"></a>API-Referenz

Suchen Sie nach der API-Referenz für diesen Dienst?

- [Azure AD Identitäts- und Management-API in Microsoft Graph v1. 0](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0)
- [Azure AD Identitäts- und Management-API in Microsoft Graph beta](/graph/api/resources/azure-ad-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Nächste Schritte

- Informationen zum [Verwenden der Azure AD-REST-APIs](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).
- Verwenden von Azure AD zum [Authentifizieren](auth-overview.md) bei Microsoft Graph.
- Integrieren der [Azure AD-Anmeldung](https://azure.microsoft.com/en-us/develop/identity/signin/) in Ihre App oder Website.
- Informationen zu Neuerungen in den Azure AD-APIs finden Sie im [Changelog](changelog.md).
- In den [Beispielen](https://developer.microsoft.com/graph/graph/examples) finden Sie weitere Ideen für die Verwendung von Microsoft Graph.
