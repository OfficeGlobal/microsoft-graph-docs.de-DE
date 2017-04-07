# <a name="known-issues-with-microsoft-graph"></a>Bekannte Probleme in Microsoft Graph

Dieser Artikel beschreibt bekannte Probleme in Microsoft Graph. Informationen zu den neuesten Updates finden Sie im [Microsoft Graph Changelog](http://graph.microsoft.io/en-us/changelog).

## <a name="graph-explorer"></a>Graph-Tester
Die Microsoft-Kontoanmeldungen beim Graph-Tester wurden aufgrund eines Dienstproblems deaktiviert. Wir arbeiten aktiv an einer Lösung und werden diesen Text aktualisieren, wenn wir soweit sind.  

Anmeldungen mit Internet Explorer und Microsoft Edge haben nicht funktioniert. Dieses Problem ist seit 2. Februar 2017 gelöst.

## <a name="users"></a>Benutzer
#### <a name="no-instant-access-after-creation"></a>Kein direkter Zugriff nach der Erstellung
Benutzer können direkt über POST in der Benutzerentität erstellt werden. Eine Office 365-Lizenz muss zunächst einem Benutzer zugewiesen werden, damit dieser Zugriff auf Office 365-Dienste erhält. Aufgrund der verteilten Art des Diensts kann es bis zu 15 Minuten dauern, bis Dateien-, Nachrichten- und Ereignisentitäten für diesen Benutzer über die Microsoft Graph-API zur Verfügung stehen. In dieser Zeit erhalten Apps als Antwort den HTTP-Fehler 404. 

#### <a name="photo-restrictions"></a>Fotoeinschränkungen
Benutzerprofilfotos können nur gelesen und aktualisiert werden, wenn der Benutzer über ein Postfach verfügt. Darüber hinaus kann auf Fotos, die *ggf.* zuvor mithilfe der **thumbnailPhoto**-Eigenschaft (unter Verwendung der Office 365 Unified-API-Vorschau oder Azure AD Graph oder über die AD Connect-Synchronisierung) gespeichert wurden, nicht mehr über die Microsoft Graph-Benutzerfotoeigenschaft zugegriffen werden. Beim Auftreten eines Fehlers beim Lesen oder Aktualisieren eines Fotos wird die folgende Meldung angezeigt:

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

 > **Hinweis**:  Kurz nach der allgemeinen Verfügbarkeit wird das Speichern und Abrufen von Benutzerprofilfotos aktiviert, selbst wenn der Benutzer über kein Postfach verfügt. Dann sollte dieser Fehler nicht mehr auftreten.


#### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Hinzufügen von und Zugreifen auf ICS-basierte Kalender im Postfach des Benutzers
Derzeit gibt es eine teilweise Unterstützung für einen Kalender, der auf einem Internet-Kalenderabonnement (ICS) basiert:

* Sie können einen ICS-basierten Kalender einem Benutzerpostfach über die Benutzeroberfläche, jedoch nicht über die Microsoft Graph-API hinzufügen. 
* [Das Auflisten der Kalender des Benutzers](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_calendars) ermöglicht Ihnen, die Eigenschaften **Name**, **Farbe** und **ID** jedes [Kalenders](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/calendar) in der Standardkalendergruppe oder einer bestimmten Kalendergruppe des Benutzers abzurufen, einschließlich ICS-basierte Kalender. Sie können die ICS-URL in der Kalenderressource nicht speichern und nicht darauf zugreifen.
* Sie haben auch die Möglichkeit zum [Auflisten der Ereignisse](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_events) eines ICS-basierten Kalenders.

## <a name="groups"></a>Gruppen
#### <a name="policy"></a>Richtlinie
Beim Erstellen und Benennen einer Office 365-Gruppe mit Microsoft Graph werden Office 365-Gruppenrichtlinien umgangen, die über Outlook Web App konfiguriert werden. 

#### <a name="group-permission-scopes"></a>Berechtigungsbereiche für Gruppen
Microsoft Graph stellt zwei Berechtigungsbereiche (*Group.Read.All* und *Group.ReadWrite.All*) für den Zugriff auf Gruppen-APIs zur Verfügung.  
Diesen Berechtigungsbereichen muss ein Administrator seine Zustimmung erteilen (Dies ist anders als in der Vorschauversion).  In Zukunft werden neue Bereiche für Gruppen hinzugefügt, für die Benutzer Ihre Zustimmung erteilen können.

Außerdem unterstützt nur die API für die Hauptgruppenadministration und -verwaltung den Zugriff mithilfe delegierter oder Nur-App-Berechtigungen. Alle anderen Features der Gruppen-API unterstützen nur delegierte Berechtigungen. 

Beispiele für Gruppenfeatures, die delegierte und Nur-App-Berechtigungen unterstützen: 

* Erstellen und Löschen von Gruppen
* Abrufen und Aktualisieren von Gruppeneigenschaften, die zur Gruppenadministration oder -verwaltung gehören
* [Verzeichniseinstellungen](../api-reference/v1.0/resources/directoryobject.md) für Gruppen, Typ und Synchronisierung
* Gruppenbesitzer und Mitgliedschaft


Beispiele für Gruppenfeatures, die nur delegierte Berechtigungen unterstützen:

* Gruppenunterhaltungen, Ereignisse, Fotos
* Externe Absender, akzeptierte oder abgelehnte Absender, Gruppenabonnement
* Benutzerfavoriten und Anzahl ungesehener Elemente


#### <a name="adding-and-getting-attachments-of-group-posts"></a>Hinzufügen und Abrufen von Anlagen von Gruppenbeiträgen
Durch das [Hinzufügen](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_post_attachments) von Anlagen zu Gruppenbeiträgen, das [Auflisten](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_list_attachments) und das Abrufen von Anlagen von Gruppenbeiträgen wird aktuell die Fehlermeldung „Die OData-Anforderung wird nicht unterstützt“ zurückgegeben. Für die `/v1.0`- und `/beta`-Versionen wurde eine Problemlösung entwickelt, die bis Ende Januar 2016 allgemein verfügbar sein sollte.


#### <a name="setting-the-allowexternalsenders-property"></a>Festlegen der allowExternalSenders-Eigenschaft
Aktuell liegt ein Problem vor, aufgrund dessen sich die Eigenschaft **allowExternalSenders** einer Gruppe in POST- oder PATCH-Operationen nicht festlegen lässt. Das Problem tritt sowohl in `/v1.0` als auch in `/beta` auf.


## <a name="contacts"></a>Kontakte

#### <a name="organization-contacts-available-in-only-beta"></a>Organisationskontakte nur in Betaversion verfügbar
Derzeit werden nur persönliche Kontakten unterstützt. Organisationskontakte werden derzeit nicht in `/v1.0` unterstützt, sind jedoch in `/beta` vorhanden.

#### <a name="default-contacts-folder"></a>Standardordner für Kontakte

In der `/v1.0`-Version enthält `GET /me/contactFolders` keinen Standardordner für Kontakte des Benutzers. 

Es wird ein Update zur Verfügung gestellt. In der Zwischenzeit können Sie die folgende [list contacts](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_contacts)-Abfrage und die **parentFolderId**-Eigenschaft als Problemumgehung verwenden, um die ID des Standardordners für Kontakte abzurufen:

```
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```
In der obigen Abfrage gilt Folgendes:
1. `/me/contacts?$top=1` ruft die Eigenschaften eines [Kontakts](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact) im Standardordner für Kontakte ab.
2. Das Anfügen von `&$select=parentFolderId` gibt nur die **parentFolderId**-Eigenschaft des Kontakts zurück, also die ID des Standardordners für Kontakte.


#### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>Zugreifen auf Kontakte über einen Kontakteordner in der Betaversion
In der Version `/beta` liegt aktuell ein Problem vor, aufgrund dessen der Zugriff auf einen [Kontakt](../api-reference/beta/resources/contact.md) über die Angabe seines übergeordneten Ordners in der REST-Anforderungs-URL in den folgenden 2 Szenarien nicht möglich ist:

* Zugreifen auf einen Kontakt über ein [contactFolder](../api-reference/beta/resources/contactfolder.md)-Objekt höchster Ebene des Benutzers
```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
* Zugreifen auf einen Kontakt in einem untergeordneten Ordner eines **contactFolder**-Objekts  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

Alternativ können Sie den Kontakt ganz einfach [per GET-Befehl abrufen](../api-reference/beta/api/contact_get.md), indem Sie seine ID wie unten gezeigt angeben. Das funktioniert, weil der Befehl „GET /contacts“ in der Version `/beta` auf alle Kontakte im Postfach des Benutzers angewendet wird:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a>Nachrichten
#### <a name="the-comment-parameter-for-creating-a-draft"></a>Der comment-Parameter für das Erstellen eines Entwurfs
Der comment-Parameter für das Erstellen eines Antwort- oder Weiterleitungsentwurfs ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) wird nicht Teil des Textkörpers des resultierenden Nachrichtenentwurfs.  


## <a name="drives-files-and-content-streaming"></a>Laufwerke, Dateien und Streamen von Inhalten
* Beim ersten Zugriff auf ein persönliches Benutzerlaufwerk über Microsoft Graph tritt ein 401-Fehler auf, wenn der Benutzer seine persönliche Website noch nicht in einem Browser aufgerufen hat.

## <a name="functionality-available-only-in-office-365-rest-apis"></a>Nur in Office 365-REST-APIs verfügbare Funktionen

Einige Funktionen sind noch nicht verfügbar in Microsoft Graph. Wenn Sie die gesuchte Funktionalität nicht finden, können Sie die endpunkt-spezifischen [Office 365 REST-APIs](https://msdn.microsoft.com/en-us/office/office365/api/api-catalog) verwenden.


#### <a name="batching"></a>Batchverarbeitung
Batchverarbeitung wird von Microsoft Graph nicht unterstützt. Sie können jedoch die Outlook-Betaendpunkte und [Outlook-REST-Batchaufrufe](https://msdn.microsoft.com/en-us/office/office365/api/batch-outlook-rest-requests) verwenden. 

#### <a name="availability-in-china"></a>Verfügbarkeit in China
Der Microsoft Graph-Dienst wird von21Vianet betrieben (und ist jetzt in China verfügbar). Lesen Sie [Unabhängige Microsoft Graph-Cloudbereitstellungen](http://developer.microsoft.com/en-us/graph/docs/overview/deployments), um weitere Informationen zu erhalten und mehr über die Einschränkungen zu erfahren.

#### <a name="service-actions-and-functions"></a>Dienstaktionen und Funktionen
`isMemberOf` und `getObjectsById` sind in Microsoft Graph nicht verfügbar.

## <a name="microsoft-graph-permissions"></a>Microsoft Graph-Berechtigungen
Neueste Informationen zu den von Microsoft Graph unterstützten Anwendungs- und delegierten Berechtigungen finden Sie im Thema [Berechtigungsbereiche](http://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes). Darüber hinaus gelten die folgenden Einschränkungen für `v1.0`:

|Berechtigung |    Berechtigungstyp | Einschränkung |    Alternative |
|-----------|-----------------|------------|--------------|
|_User.ReadWrite_| Delegated    | Mobiltelefonnummer kann nicht aktualisiert werden.|    Wählen Sie auch `Directory.AccessAsUser.All`| 
|_User.ReadWrite.All_|    Delegated|    Es können keine anderen CRUD-Vorgänge für `User` ausgeführt werden als das Aktualisieren des HD-Fotos vom Benutzer und der erweiterten Profileigenschaften.|    Wählen Sie `Directory.ReadWrite.All` oder `Directory.AccessAsUser.All`, wenn Löschen von Benutzern erforderlich ist.|
|_User.Read.All_|    Application    |Es können keine Lesevorgänge für andere Benutzer ausgeführt werden.|    Wählen Sie auch `Directory.Read.All`|
| _User.ReadWrite.All_ |    Application |    Es können keine anderen CRUD-Vorgänge für `User` ausgeführt werden als das Aktualisieren des HD-Fotos vom Benutzer und der erweiterten Profileigenschaften. |    Wählen Sie auch `Directory.ReadWrite.All`. **HINWEIS**: Löschen von Benutzern ist nicht möglich.|
|_Group.Read.All_    | Application |    Gruppen oder Gruppenmitgliedschaften können nicht aufgelistet werden.  Gruppeninhalte können weiterhin für Office-Gruppen gelesen werden.	    | Wählen Sie auch `Directory.Read.All` |
|_Group.ReadWrite.All_    | Application    | Auflisten von Gruppen oder Gruppenmitgliedschaften, Erstellen von Gruppen, Aktualisieren von Gruppenmitgliedschaften oder Löschen von Gruppen ist nicht möglich.  Gruppeninhalte können weiterhin für Office-Gruppen gelesen und aktualisiert werden.	    | Wählen Sie auch `Directory.ReadWrite.All`. **HINWEIS**:  Löschen von Gruppen ist nicht möglich.|

Darüber hinaus gelten die folgenden `/beta`-Einschränkungen:

|Berechtigung |    Berechtigungstyp | Einschränkung |    Alternative |
|-----------|-----------------|------------|--------------|
| _Group.ReadWrite.All_    | Delegated    | Planeraufgaben können in Office-Gruppen nicht gelesen oder aktualisiert werden.	    | Wählen Sie auch `Tasks.ReadWrite`|
|_Tasks.ReadWrite_    | Delegated    | Aufgaben von angemeldeten Benutzern können nicht gelesen oder aktualisiert werden.| Wählen Sie auch `Group.ReadWrite.All`|

## <a name="odata-related-limitations"></a>OData-bezogene Einschränkungen
* **$expand**-Einschränkungen: 
 * Keine Unterstützung für `nextLink`.
 * Keine Unterstützung für mehr als eine Erweiterungsebene.
 * Keine Unterstützung mit zusätzlichen Parametern (**$filter**, **$select**).
* Mehrere Namespaces werden nicht unterstützt.
* GET-Anforderungen für `$ref` und Umwandlung wird für Benutzer, Gruppen, Geräte, Dienstprinzipale und Anwendungen nicht unterstützt.
* `@odata.bind` wird nicht unterstützt.  Ein Entwickler kann daher `Accepted` oder `RejectedSenders` für eine Gruppe nicht ordnungsgemäß festlegen.
* `@odata.id` ist bei Nicht-Aufnahmenavigationen (z. B. Nachrichten) nicht vorhanden, wenn minimale Metadaten verwendet werden.
* Arbeitsauslastungsübergreifende Filter/Suche ist nicht verfügbar. 
* Volltextsuche (unter Verwendung von **$search**) ist nur für einige Entitäten wie Nachrichten verfügbar.

  >  Ihr Feedback ist uns wichtig. Nehmen Sie auf [Stack Overflow](http://stackoverflow.com/questions/tagged/office365) Kontakt mit uns auf. Taggen Sie Ihre Fragen mit {MicrosoftGraph} und {office365}.


