# <a name="working-with-education-apis-in-microsoft-graph"></a>Arbeiten mit Education-APIs in Microsoft Graph

Mit Education-APIs in Microsoft Graph werden Office 365-Ressourcen und -Daten mithilfe von Informationen optimiert, die für Bildungsszenarien, u. a. Schulen, Schüler, Studenten, Lehrer, Kurse und Anmeldungen relevant sind. Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.

Education-APIs umfassen Ressourcen für Listenerstellung und Zuordnungen, die Sie für die Kommunikation mit Listenerstellungsdiensten in Microsoft Teams verwenden können. Sie können diese Ressourcen zum Verwalten von Schulplänen verwenden.

## <a name="authorization"></a>Autorisierung

Damit die Education-APIs in Microsoft Graph aufgerufen werden können, muss Ihre App ein Zugriffstoken erwerben. Weitere Informationen zu Zugriffstoken finden Sie unter [Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph](https://developer.microsoft.com/de-DE/graph/docs/concepts/auth_overview). Zudem muss Ihre App über die entsprechenden Berechtigungen verfügen. Weitere Informationen finden Sie unter [Education-Berechtigungen](../../../concepts/permissions_reference.md#education-permissions). 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>App-Berechtigungen zum Aktivieren der Zustimmung von Schul-IT-Administratoren 

Um Apps bereitzustellen, die in Education-APIs in Microsoft Graph integriert sind, müssen Schul-IT-Administratoren zunächst ihre Zustimmung für die von der App angeforderten Berechtigungen erteilen. Diese Zustimmung muss nur einmal erteilt werden, sofern sich die Berechtigungen nicht ändern. Nachdem der Administrator seine Zustimmung erteilt hat, wird die App für alle Benutzer im Mandanten bereitgestellt.

Verwenden Sie den folgenden REST-Aufruf, um ein Dialogfeld für die Zustimmung anzuzeigen.

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

- [Auflisten aller Schulen](../api/educationroot_list_schools.md) 
- [Auflisten von Schulen, in denen ein Kurs unterrichtet wird](../api/educationclass_list_schools.md)
- [Auflisten von Schulen für einen Benutzer](../api/educationuser_list_schools.md)
- [Abrufen aller Kurse](../api/educationroot_list_classes.md )
- [Abrufen von Kursen einer Schule](../api/educationschool_list_classes.md)
- [Auflisten von Kursen für einen Benutzer](../api/educationuser_list_classes.md)
- [Hinzufügen von Kursen zu einer Schule](../api/educationschool_post_classes.md)
- [Abrufen von Schülern/Studenten und Lehrern für einen Kurs](../api/educationclass_list_members.md)
- [Hinzufügen von Mitgliedern zu einem Kurs](../api/educationclass_post_members.md) 
- [Auflisten von Lehrern für einen Kurs](../api/educationclass_list_teachers.md)
- [Abrufen von Benutzern in einer Schule](../api/educationschool_list_users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="next-steps"></a>Nächste Schritte
Verwenden Sie die Microsoft Graph-Education-APIs zum Erstellen von Lösungen für Bildungseinrichtungen, die auf Schulpläne zugreifen. So erhalten Sie weitere Informationen:

- Erfahren Sie, welche Ressourcen und Methoden für Ihr Szenario am besten geeignet sind.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/de-DE/graph/graph-explorer) aus.

