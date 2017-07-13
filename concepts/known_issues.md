# Bekannte Probleme in Microsoft Graph
<a id="known-issues-with-microsoft-graph" class="xliff"></a>

Dieser Artikel beschreibt bekannte Probleme in Microsoft Graph. Informationen zu den neuesten Updates finden Sie im [Microsoft Graph-Änderungsprotokoll](changelog.md).

## Benutzer
<a id="users" class="xliff"></a>

### Kein direkter Zugriff nach der Erstellung
<a id="no-instant-access-after-creation" class="xliff"></a>

Benutzer können direkt über POST in der Benutzerentität erstellt werden. Eine Office 365-Lizenz muss zunächst einem Benutzer zugewiesen werden, damit dieser Zugriff auf Office 365-Dienste erhält. Aufgrund der verteilten Art des Diensts kann es bis zu 15 Minuten dauern, bis Dateien-, Nachrichten- und Ereignisentitäten für diesen Benutzer über die Microsoft Graph-API zur Verfügung stehen. In dieser Zeit erhalten Apps als Antwort den HTTP-Fehler 404.

### Fotoeinschränkungen
<a id="photo-restrictions" class="xliff"></a>

Benutzerprofilfotos können nur gelesen und aktualisiert werden, wenn der Benutzer über ein Postfach verfügt. Darüber hinaus kann auf Fotos, die *ggf.* zuvor mithilfe der **thumbnailPhoto**-Eigenschaft (unter Verwendung der Office 365 Unified-API-Vorschau oder Azure AD Graph oder über die AD Connect-Synchronisierung) gespeichert wurden, nicht mehr über die Microsoft Graph-Eigenschaft **photo** der [user](../api-reference/v1.0/resources/user.md)-Ressource zugegriffen werden. Beim Auftreten eines Fehlers beim Lesen oder Aktualisieren eines Fotos wird die folgende Meldung angezeigt:

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### Verwenden der Delta-Abfrage
<a id="using-delta-query" class="xliff"></a>

Bekannte Probleme bei der Verwendung der Delta-Abfrage finden Sie im Abschnitt [Delta-Abfrage](#delta-query) in diesem Artikel.

## Gruppen und Microsoft Teams
<a id="groups-and-microsoft-teams" class="xliff"></a>

>**Hinweis** Microsoft Teams ist derzeit nur im Beta-Endpunkt von Microsoft Graph als Vorschauversion verfügbar.

### Richtlinie
<a id="policy" class="xliff"></a>

Beim Erstellen und Benennen einer Office 365-Gruppe mit Microsoft Graph werden Office 365-Gruppenrichtlinien umgangen, die über Outlook Web App konfiguriert werden. 

### Berechtigungen für Gruppen und Microsoft Teams
<a id="permissions-for-groups-and-microsoft-teams" class="xliff"></a>

Microsoft Graph stellt zwei Berechtigungen (*Group.Read.All* und *Group.ReadWrite.All*) für den Zugriff auf Gruppen und Microsoft Teams zur Verfügung. Diesen Berechtigungen muss ein Administrator seine Zustimmung erteilen (anders als in der Vorschauversion).  In Zukunft sollen neue Berechtigungen für Gruppen und Teams hinzugefügt werden, für die Benutzer ihre Zustimmung erteilen können.

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

### Teams in Microsoft Teams (Vorschau)
<a id="teams-in-microsoft-teams-preview" class="xliff"></a>

Microsoft Teams und Office 365-Gruppen haben eine ähnliche Funktionalität. Alle Gruppen-APIs können für Teams verwendet werden, mit der Ausnahme, dass mit der API „Gruppe erstellen“ derzeit kein Team erstellt werden kann.  In zukünftigen API-Versionen wird dies unterstützt.

### Microsoft Teams-Kanäle (Vorschau)
<a id="microsoft-teams-channels-preview" class="xliff"></a>

Zurzeit können Sie Kanäle lesen und erstellen, aber nicht aktualisieren oder löschen.  In zukünftigen API-Versionen wird dies unterstützt.

### Microsoft Teams-Chatthreads und -Chatnachrichten (Vorschau)
<a id="microsoft-teams-chat-threads-and-chat-messages-preview" class="xliff"></a>

Zurzeit können Sie Chatthreads in Kanälen erstellen, aber keine vorhandenen Chatthreads lesen und keine Antworten auf diese hinzufügen. Außerdem können Sie keine direkten Chats zwischen Benutzern lesen oder schreiben, die sich außerhalb des Bereichs eines Teams oder Kanals befinden.  Zukünftige API-Versionen werden über zusätzliche Funktionen in diesem Bereich verfügen.


### Hinzufügen und Abrufen von Anlagen von Gruppenbeiträgen
<a id="adding-and-getting-attachments-of-group-posts" class="xliff"></a>

Durch das [Hinzufügen](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_post_attachments) von Anlagen zu Gruppenbeiträgen, das [Auflisten](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_list_attachments) und das Abrufen von Anlagen von Gruppenbeiträgen wird aktuell die Fehlermeldung „Die OData-Anforderung wird nicht unterstützt“ zurückgegeben. Für die `/v1.0`- und `/beta`-Versionen wurde eine Problemlösung entwickelt, die bis Ende Januar 2016 allgemein verfügbar sein sollte.

### Festlegen der allowExternalSenders-Eigenschaft
<a id="setting-the-allowexternalsenders-property" class="xliff"></a>

Aktuell liegt ein Problem vor, aufgrund dessen sich die Eigenschaft **allowExternalSenders** einer Gruppe in POST- oder PATCH-Operationen nicht festlegen lässt. Das Problem tritt sowohl in `/v1.0` als auch in `/beta` auf.

### Verwenden der Delta-Abfrage
<a id="using-delta-query" class="xliff"></a>

Bekannte Probleme bei der Verwendung der Delta-Abfrage finden Sie im Abschnitt [ Delta-Abfrage](#delta-query) in diesem Artikel.


## Kalender
<a id="calendars" class="xliff"></a>

### Hinzufügen von und Zugreifen auf ICS-basierte Kalender im Postfach des Benutzers
<a id="adding-and-accessing-ics-based-calendars-in-users-mailbox" class="xliff"></a>

Derzeit gibt es eine teilweise Unterstützung für einen Kalender, der auf einem Internet-Kalenderabonnement (ICS) basiert:

* Sie können einen ICS-basierten Kalender einem Benutzerpostfach über die Benutzeroberfläche, jedoch nicht über die Microsoft Graph-API hinzufügen.
* [Das Auflisten der Kalender des Benutzers](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_calendars) ermöglicht Ihnen, die Eigenschaften **name**, **color** und **id** jedes [Kalenders](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/calendar) in der Standardkalendergruppe des Benutzers oder einer bestimmten Kalendergruppe abzurufen, einschließlich ICS-basierte Kalender. Sie können die ICS-URL in der Kalenderressource nicht speichern und nicht darauf zugreifen.
* Sie haben auch die Möglichkeit zum [Auflisten der Ereignisse](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_events) eines ICS-basierten Kalenders.

### Zugreifen auf einen freigegebenen Kalender
<a id="accessing-a-shared-calendar" class="xliff"></a>

Beim Versuch, auf Ereignisse in einem Kalender zuzugreifen, der von einem anderen Benutzer mithilfe des folgenden Vorgangs freigegeben wurde:

```http
GET \users('{id}')\calendars('{id}')\events
```

Möglicherweise wird HTTP 500 mit dem Fehlercode `ErrorInternalServerTransientError` angezeigt. Der Fehler tritt aus folgendem Grund auf:

- Bisher gibt es zwei Methoden zur Implementierung der Kalenderfreigabe, die zur Unterscheidung einmal als der „alte“ Implementierungsansatz und einmal als der „neue“ Implementierungsansatz bezeichnet werden.
- Der neue Ansatz ist derzeit für die Kalenderfreigabe mit Berechtigungen zum Anzeigen oder Bearbeiten verfügbar, jedoch nicht mit  aber nicht mit Berechtigungen der Stellvertretung. 
- Sie können die Kalender-REST-API verwenden, um freigegebene Kalender anzuzeigen oder freizugeben, aber nur, wenn die Kalender auf die **neue** Weise freigegebenen wurden. 
- Sie können die Kalender-REST-API nicht verwenden, um freigegebene Kalender (oder deren Ereignisse) anzuzeigen oder freizugeben, wenn die Kalender auf die **alte** Weise freigegebenen wurden.


Wenn ein Kalender mit Berechtigungen zum Anzeigen oder Bearbeiten auf die alte Weise freigegeben wurde, können Sie dieses Problem umgehen und die Kalenderfreigabe für die Verwendung des neuen Ansatzes aktualisieren. Im Laufe der Zeit werden alle freigegebenen Kalender für die Verwendung des neuen Ansatzes automatisch in Outlook aktualisiert, einschließlich mit Berechtigungen der Stellvertretung freigegebener Kalender. 

Gehen Sie folgendermaßen vor, um einen freigegebenen Kalender für die Verwendung des neuen Ansatzes manuell zu aktualisieren:
1.  Der Empfänger entfernt den Kalender, der zuvor für diesen freigegeben wurde.
2.  Der Besitzer des Kalenders gibt den Kalender erneut in Outlook im Web, Outlook für iOS oder Outlook für Android frei.
3.  Der Empfänger akzeptiert den freigegebenen Kalender mithilfe von Outlook im Web erneut. (Zukünftig können auch andere Outlook-Clients verwendet werden.)
4.  Der Empfänger überprüft, ob der Kalender auf die neue Weise erfolgreich erneut freigegeben wurde und in Outlook für iOS oder in Outlook für Android angezeigt werden kann.

Ein für Sie mit dem neuen Ansatz freigegebener Kalender wird genau wie jeder andere Kalender in Ihrem Postfach angezeigt. Sie können die Kalender-REST-API verwenden, um Ereignisse im freigegebenen Kalender so anzuzeigen oder zu bearbeiten, als wäre es Ihr eigener Kalender. Beispiel:

```http
GET \me\calendars('{id}')\events
```


## Kontakte
<a id="contacts" class="xliff"></a>

### Organisationskontakte nur in Betaversion verfügbar
<a id="organization-contacts-available-in-only-beta" class="xliff"></a>

Derzeit werden nur persönliche Kontakten unterstützt. Organisationskontakte werden derzeit nicht in `/v1.0` unterstützt, sind jedoch in `/beta` vorhanden.

### Standardordner für Kontakte
<a id="default-contacts-folder" class="xliff"></a>

In der `/v1.0`-Version enthält `GET /me/contactFolders` keinen Standardordner für Kontakte des Benutzers. 

Es wird ein Update zur Verfügung gestellt. In der Zwischenzeit können Sie die folgende [list contacts](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_contacts)-Abfrage und die **parentFolderId**-Eigenschaft als Problemumgehung verwenden, um die ID des Standardordners für Kontakte abzurufen:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

In der obigen Abfrage gilt Folgendes:

1. `/me/contacts?$top=1` ruft die Eigenschaften eines [Kontakts](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact) im Standardordner für Kontakte ab.
2. Das Anfügen von `&$select=parentFolderId` gibt nur die **parentFolderId**-Eigenschaft des Kontakts zurück, also die ID des Standardordners für Kontakte.


### Zugreifen auf Kontakte über einen Kontakteordner in der Betaversion
<a id="accessing-contacts-via-a-contact-folder-in-beta" class="xliff"></a>

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

## Nachrichten
<a id="messages" class="xliff"></a>

### Der comment-Parameter für das Erstellen eines Entwurfs
<a id="the-comment-parameter-for-creating-a-draft" class="xliff"></a>

Der comment-Parameter für das Erstellen eines Antwort- oder Weiterleitungsentwurfs ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) wird nicht Teil des Textkörpers des resultierenden Nachrichtenentwurfs.  

## Laufwerke, Dateien und Streamen von Inhalten
<a id="drives-files-and-content-streaming" class="xliff"></a>

* Beim ersten Zugriff auf ein persönliches Benutzerlaufwerk über Microsoft Graph tritt ein 401-Fehler auf, wenn der Benutzer seine persönliche Website noch nicht in einem Browser aufgerufen hat.

## Einschränkungen für Abfrageparameter
<a id="query-parameter-limitations" class="xliff"></a>

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

## Delta-Abfrage
<a id="delta-query" class="xliff"></a>

* OData-Kontext wird beim Nachverfolgen von Änderungen an Beziehungen manchmal falsch zurückgegeben.
* Schemaerweiterungen (Legacy) werden nicht mit $select-Anweisung, sondern ohne $select zurückgegeben.
* Clients können keine Änderungen an offenen Erweiterungen oder registrierten Schemaerweiterungen nachverfolgen.

## Änderungen an der application- und servicePrincipal-API
<a id="application-and-serviceprincipal-api-changes" class="xliff"></a>

Es gibt Änderungen an den [application](../api-reference/beta/resources/application.md)- und [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md)-Entitäten, die derzeit entwickelt werden. Nachfolgend finden Sie eine Zusammenfassung aktueller Einschränkungen und API-Features, die derzeit entwickelt werden.

Aktuelle Einschränkungen:

* Einige Anwendungseigenschaften (z. B. appRoles und addIns) sind erst verfügbar, wenn alle Änderungen abgeschlossen sind.
* Es können nur Apps mit mehreren Mandanten registriert werden.
* Das Aktualisieren von Apps ist auf Apps beschränkt, die nach dem anfänglichen Beta-Update registriert wurden.
* Azure Active Directory-Benutzer können Apps registrieren und weitere Besitzer hinzufügen.
* Unterstützung für OpenID Connect und OAuth-Protokolle.
* Richtlinienzuweisungen zu einer App schlagen fehl. 
* Vorgänge mit ownedObjects, die die appId erfordern, schlagen fehl (z. B. users/{id|userPrincipalName}/ownedObjects/{id}/...).

In der Entwicklung:

* Die Möglichkeit, Apps mit nur einem Mandanten zu registrieren.
* Updates für servicePrincipal.
* Migration von vorhandenen Azure AD-Apps zum aktualisierten Modell.
* Unterstützung für appRoles, vorab autorisierte Clients, optionale Ansprüche, Gruppenmitgliedschaftsansprüche und Branding
* Benutzer eines Microsoft-Kontos (MSA-Benutzer) können Apps registrieren.
* Unterstützung für SAML und WsFed-Protokolle.

## Erweiterungen
<a id="extensions" class="xliff"></a>

### Die Änderungsnachverfolgung wird nicht unterstützt.
<a id="change-tracking-is-not-supported" class="xliff"></a>

Die Änderungsnachverfolgung (Delta-Abfrage) wird für Eigenschaften von offenen Erweiterungen oder Schemaerweiterungen nicht unterstützt.

### Gleichzeitiges Erstellen einer Ressource und einer offenen Erweiterung
<a id="creating-a-resource-and-open-extension-at-the-same-time" class="xliff"></a>

Wenn Sie eine Instanz von Ressourcen des Typs **administrativeUnit**, **device**, **group**, **organization** oder **user** erstellen, können Sie nicht gleichzeitig eine offene Erweiterung angeben. Sie müssen zuerst die Instanz erstellen und dann eine ``POST``-Anforderung auf diese Instanz anwenden, in der Sie die Daten der offenen Erweiterung angeben.

### Grenzwert von 100 zulässigen Werten für Schemaerweiterungseigenschaften pro Ressourceninstanz.
<a id="limit-of-100-schema-extension-property-values-allowed-per-resource-instance" class="xliff"></a>

Für Verzeichnisressourcen wie **device**, **group** und **user** gilt aktuell: Für eine Ressourceninstanz dürfen maximal 100 Eigenschaftswerte von Schemaerweiterungen festgelegt werden.

## JSON-Batchverarbeitung
<a id="json-batching" class="xliff"></a>

### Keine geschachtelter Batch
<a id="no-nested-batch" class="xliff"></a>

JSON-Batchanforderungen dürfen keine geschachtelten Batchanforderungen enthalten.

### Alle einzelnen Anforderungen müssen synchron sein.
<a id="all-individual-requests-must-be-synchronous" class="xliff"></a>

Alle in einer Batchanforderung enthaltenen Anforderungen müssen synchron ausgeführt werden. Falls vorhanden, wird die `respond-async`-Präferenz ignoriert.

### Keine Transaktionen
<a id="no-transactions" class="xliff"></a>

Microsoft Graph unterstützt derzeit keine Transaktionsverarbeitung von einzelnen Anforderungen. Die `atomicityGroup`-Eigenschaft von einzelnen Anforderungen wird ignoriert.

### URIs müssen relativ sein
<a id="uris-must-be-relative" class="xliff"></a>

Geben Sie in Batchanforderungen immer relative URIs an. Microsoft Graph macht daraus dann mithilfe des in der Batch-URL enthaltenen Versionsendpunkts absolute URLs.

### Beschränkung der Batchgröße
<a id="limit-on-batch-size" class="xliff"></a>

JSON-Batchanforderungen sind derzeit auf fünf einzelne Anforderungen beschränkt. In der weiteren Entwicklung der JSON-Batchverarbeitung wird dieser Grenzwert hochgesetzt.

### Vereinfachte Abhängigkeiten
<a id="simplified-dependencies" class="xliff"></a>

Einzelne Anforderungen können von anderen einzelnen Anforderungen abhängen. Derzeit können Anforderungen nur von einer einzigen anderen Anforderung abhängen und müssen einem der folgenden drei Muster entsprechen:

1. Parallel: Eine einzelne Anforderung gibt eine Abhängigkeit in der `dependsOn`-Eigenschaft an.
2. Seriell: Alle einzelnen Anforderungen hängen von der vorherigen einzelnen Anforderung ab.
3. Gleich: Alle einzelnen Anforderungen, die eine Abhängigkeit in der `dependsOn`-Eigenschaft angeben, geben die gleiche Abhängigkeit an.

In der weiteren Entwicklung der JSON-Batchverarbeitung werden diese Einschränkungen entfernt.

## Apps vom Cloudlösungsanbieter
<a id="cloud-solution-provider-apps" class="xliff"></a>

### Apps vom Cloudlösungsanbieter müssen den Azure AD-Endpunkt verwenden
<a id="csp-apps-must-use-azure-ad-endpoint" class="xliff"></a>

CSP-Apps (Cloud-Lösungsanbieter) müssen Token von den Azure AD (v1)-Endpunkten erwerben, um Microsoft Graph erfolgreich in ihren partnerverwalteten Kunden aufrufen zu können. Derzeit wird der Erwerb eines Tokens über den neueren Azure AD v2.0-Endpunkt nicht unterstützt.

### Eine Vorabgenehmigung für Apps vom Cloudlösungsanbieter funktioniert bei einigen Kundenmandanten nicht
<a id="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants" class="xliff"></a>

Unter bestimmten Umständen funktioniert die Vorabgenehmigung für Apps vom Cloudlösungsanbieter bei einigen Kundenmandanten nicht.

- Für Apps, die delegierte Berechtigungen verwenden, wird bei der ersten Verwendung der App mit einem neuen Kundenmandanten möglicherweise der folgende Fehler nach der Anmeldung angezeigt: `AADSTS50000: There was an error issuing a token`.
- Für Apps, die Anwendungsberechtigungen verwenden, kann Ihre App ein Token erfassen, beim Aufrufen von Microsoft Graph wird jedoch unerwartet die Meldung angezeigt, dass der Zugriff verweigert wurde.

Wir arbeiten daran, dieses Problem so schnell wie möglich zu lösen, damit die Vorabgenehmigung für alle Kundenmandanten funktioniert.

In der Zwischenzeit können Sie die folgende Problemumgehung verwenden, um die Entwicklung und das Testen nicht zu blockieren.

>**HINWEIS:** Dies ist keine dauerhafte Lösung und soll nur dazu dienen, die Entwicklung nicht zu blockieren.  Diese Problemumgehung ist nicht mehr erforderlich, nachdem das zuvor erwähnte Problem behoben wurde.  Diese Problemumgehung muss nicht rückgängig gemacht werden, nachdem die Korrektur vorhanden ist.

1. Öffnen Sie eine Azure AD v2-PowerShell-Sitzung, und stellen Sie eine Verbindung mit Ihrem `customer`-Mandanten her, indem Sie Ihre Administrator-Anmeldeinformationen in das Anmeldefenster eingeben. Sie können Azure AD PowerShell V2 [hier](https://www.powershellgallery.com/packages/AzureAD) herunterladen und installieren.

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Erstellen Sie den Microsoft Graph-Dienstprinzipal.

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## Nur in Office 365-REST- oder Azure AD-Graph-APIs verfügbare Funktionen
<a id="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis" class="xliff"></a>

Einige Funktionen sind in Microsoft Graph noch nicht verfügbar. Wenn Sie die gesuchte Funktion nicht finden, können Sie die endpunktspezifischen [Office 365-REST-APIs](https://msdn.microsoft.com/en-us/office/office365/api/api-catalog) verwenden. Für Azure Active Directory finden Sie im Blogbeitrag [Microsoft Graph oder Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) Informationen über die Features, die nur über die Azure AD-Graph-API verfügbar sind.

## Feedback
<a id="feedback" class="xliff"></a>

> Ihr Feedback ist uns wichtig. Nehmen Sie unter [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph) Kontakt mit uns auf.
