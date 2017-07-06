# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Arbeiten mit Active Directory-Ressourcen in Microsoft Graph

Mit Microsoft Graph können Sie auf [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis)-Ressourcen zugreifen, die Sie für unterschiedliche Szenarien verwenden können. Dies umfasst das Verwalten von Administratorrollen (Verzeichnisrollen), das Einladen externer Benutzer zu einer Organisation, wenn Sie ein [Cloud-Lösungsanbieter (CSP) sind](https://partner.microsoft.com/cloud-solution-provider), und das Verwalten der Daten Ihrer Kunden. Microsoft Graph bietet auch verschiedene Methoden, die von vielen Arten von Apps verwendet werden können. Beispielsweise, um Informationen über transitive Gruppen- und Rollenmitgliedschaften von Benutzern zu ermitteln. 

> **Hinweis**: Einige Azure AD-Ressourcen sind in anderen Abschnitten der API-Referenz dokumentiert. Weitere Informationen finden Sie unter [Benutzer](users.md) und [Gruppen](group.md).


## <a name="authorization"></a>Autorisierung
 
Zum Aufrufen der Microsoft Graph-APIs in Azure AD-Ressourcen benötigt Ihre App die entsprechenden Berechtigungen.  Viele der APIs, die in Azure AD-Ressourcen verfügbar gemacht werden, erfordern eine der [ _Verzeichnis_berechtigungen](../../../concepts/permissions_reference.md#directory-permissions).  _Verzeichnis_berechtigungen verfügen über hohe Berechtigungen und müssen immer vom Administrator genehmigt werden. 

Es gibt zwei Arten von Berechtigungen: delegierte Berechtigungen und Anwendungsberechtigungen. Wenn Ihre App eine API im Namen eines Benutzers aufruft, benötigt sie delegierte Berechtigungen. Wenn sie eine API selbst ohne angemeldeten Benutzer aufruft, benötigt sie Anwendungsberechtigungen. Letzteres ist im Allgemeinen bei Back-End-Diensten oder Daemons der Fall. Weitere Informationen zu delegierten Berechtigungen und Anwendungsberechtigungen finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md). 

Wenn Ihre App schließlich im Namen eines Benutzers arbeitet, muss dieser Benutzer ein Mitglied einer entsprechenden [Administratorrolle](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) sein, damit Ihre App viele der Azure AD-APIs erfolgreich aufrufen kann.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle 

In der folgenden Tabelle sind einige allgemeine Szenarien aufgeführt, für die Azure AD-Ressourcen verwendet werden können.

| Anwendungsfälle        | REST-Ressourcen | Siehe auch |
|:---------------|:--------|:----------|
| **Verzeichnisobjekt und Methoden** | | |
| `directoryObject` ist die Basisklasse, von der viele Verzeichnisressourcen, z. B. Benutzer und Gruppen, erben. Microsoft Graph macht mehrere Methoden verfügbar, die Sie verwenden können, um Informationen über Benutzer, Gruppen und andere Verzeichnisobjekte zu ermitteln. Sie können beispielsweise eine transitive Mitgliedschaft in einer Liste von Gruppen überprüfen, alle Gruppen und Verzeichnisrollen zurückgeben, von denen ein Verzeichnisobjekt ein transitives Mitglied ist, oder alle Ressourcen eines bestimmten Typs (z. B. Benutzer oder Gruppe) aus einer Liste allgemeiner Ressourcen-IDs abrufen. | [directoryObject](../resources/directoryobject.md) | Nicht zutreffend |
| **Verwalten von Verzeichnisrollen (Administratorrollen)** | | |
| Aktivieren Sie Verzeichnisrollen in einem Azure AD-Mandanten, und verwalten Sie Benutzermitgliedschaften in Verzeichnisrollen. Verzeichnisrollen werden auch als „Administratorrollen“ bezeichnet. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | Weitere Informationen zu Verzeichnisrollen (Administratorrollen) finden Sie unter [Zuweisen von Administratorrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles). |
| **Verwalten von Geräten** | | |
| Verwalten Sie Geräte, die in der Organisation registriert sind. Geräte sind für Benutzer registriert und umfassen Elemente wie Laptops, Desktops, Tablets und Mobiltelefone. Geräte werden in der Regel mithilfe des Geräteregistrierungsdiensts oder von Microsoft Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. | [device](../resources/device.md) | Weitere Informationen zum Geräteregistrierungsdienst finden Sie unter [Erste Schritte mit der Azure Active Directory-Geräteregistrierung](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview).<br/><br/> Weitere Informationen zu Microsoft Intune finden Sie unter [Was ist InTune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune) und [Registrieren von Geräten für die Verwaltung in InTune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune). |
| **Verwaltung von Partnermandanten** | | |
| Abrufen von Informationen über Partnerschaften mit Kundenmandanten. | [contract](../resources/contract.md) | Ist nur in Partnermandanten vorhanden. Partnermandanten sind Azure AD-Mandanten, die zu Microsoft-Partnern gehören, die Teil der Partnerprogramme [Microsoft Cloud-Lösungsanbieter](https://partnercenter.microsoft.com/partner/programs), Office 365 Syndication oder Microsoft Advisor sind. <br/><br/>Weitere Informationen zum Verwalten von Kundendaten über Microsoft Graph als Cloud-Lösungsanbieter finden Sie unter [Aufrufen von Microsoft Graph aus einer Anwendung eines Cloud-Lösungsanbieters](../../../concepts/auth_cloudsolutionprovider.md). |
| Verwalten von Domänen, die einem Mandanten zugeordnet sind. Mithilfe von Domänenvorgängen können Registrierungsstellen die Domänenzuweisung für Dienste wie Office 365 automatisieren. | [domain](../resources/domain.md) | Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Domänennamens zum Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal). |
| **Verwaltung von Mandanten** | | |
| Rufen Sie Informationen über eine Organisation ab, z. B. die Unternehmensadresse, Kontakte für technische Fragen und Benachrichtigungen, die Dienstpläne, die die Organisation abonniert hat, sowie die Domänen, die mit dieser verknüpft sind. | [organization](../resources/organization.md) | Nicht zutreffend |
| Ruft Informationen zu den Dienst-SKUs ab, die ein Unternehmen abonniert hat. | [subscribedSku](../resources/subscribedsku.md) | Nicht zutreffend |
| Einladen externer (Gast)Benutzer zu einer Organisation. | [invitation](../resources/invitation.md) | Weitere Informationen finden Sie unter [Was ist die Azure AD B2B-Zusammenarbeit?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b). |



## <a name="next-steps"></a>Nächste Schritte
Verzeichnisressourcen und APIs können Ihnen neue Möglichkeiten eröffnen, über die Sie mit Benutzer in Kontakt treten und ihre Erfahrungen mit Microsoft Graph kontrollieren können: 

- Informieren Sie sich ausführlicher über die Methoden und Eigenschaften der Ressourcen, die für Ihr Szenario am hilfreichsten sind.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).

