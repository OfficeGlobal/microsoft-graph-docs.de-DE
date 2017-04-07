# <a name="add-custom-data-to-resources-using-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen

Microsoft Graph stellt einen zentralen API-Endpunkt bereit, der Ihnen über verschiedene Ressourcen wie [user](../api-reference/beta/resources/user.md) und [message](../api-reference/beta/resources/message.md) Zugriff auf umfassende personenzentrierte Daten und Erkenntnisse ermöglicht. Jetzt können Sie Microsoft Graph um eigene Anwendungsdaten _**erweitern**_. Sie können Microsoft Graph-Ressourcen benutzerdefinierte Eigenschaften hinzufügen, ohne dass dafür ein externer Datenspeicher nötig wäre. So könnten Sie sich beispielsweise entscheiden, Ihre App schlank zu halten und App-spezifische Benutzerprofildaten in Microsoft Graph zu speichern, indem Sie die Ressource **user** erweitern. Alternativ könnten Sie den vorhandenen Benutzerprofilspeicher Ihrer App auch beibehalten und der Ressource **user** einfach einen App-spezifischen Speicherbezeichner hinzufügen.

Microsoft Graph bietet zwei Arten von Erweiterungen. Wählen Sie den Erweiterungstyp aus, der Ihren Anwendungsanforderungen am besten entspricht:

*  **Offene Erweiterungen**: Dieser Erweiterungstyp ist ideal für die ersten Schritte mit Erweiterungen.
*  **Schemaerweiterungen**: Bei diesem Erweiterungstyp handelt es sich um einen flexibleren Mechanismus für Entwickler, die typisierte Daten speichern, ihr Schema erkennbar und gemeinsam nutzbar machen, Filteroptionen nutzen und später auch Autorisierung und die Überprüfung von Eingabedaten implementieren möchten.

>**Wichtig:** Sie sollten Erweiterungen nicht zur Speicherung vertraulicher personenbezogener Informationen wie Kontoanmeldeinformationen, Behördenkennnummern, Karteninhaberdaten, Bankkontonummern, Krankendaten oder vertraulichen Hintergrundinformationen verwenden.

## <a name="supported-resources"></a>Unterstützte Ressourcen

In der folgenden Tabelle wird die aktuelle Unterstützung für offene Erweiterungen und Schemaerweiterungen aufgeführt und angegeben, ob diese allgemein (GA/v1.0 und /beta) oder nur in der Vorschau (/beta) verfügbar sind. 

| Ressource | Offene Erweiterungen | Schemaerweiterungen |
|---------------|-------|-------|
| [Administrative Einheit](../api-reference/beta/resources/administrativeunit.md) | Nur Vorschau | Bald verfügbar |
|  [Kalenderereignis](../api-reference/beta/resources/event.md) | Allgemein verfügbar | Nur Vorschau |
|  [Kalenderereignis](../api-reference/beta/resources/event.md) für Gruppe | Allgemein verfügbar | Nur Vorschau |
|  Unterhaltungsthread der Gruppe [posten](../api-reference/beta/resources/post.md) | Allgemein verfügbar | Nur Vorschau |
|  [Gerät](../api-reference/beta/resources/device.md) | Nur Vorschau | Nur Vorschau |
|  [Gruppe](../api-reference/beta/resources/group.md) | Nur Vorschau | Nur Vorschau |
|  [Nachricht](../api-reference/beta/resources/message.md) | Allgemein verfügbar | Nur Vorschau |
|  [Organisation](../api-reference/beta/resources/organization.md) | Nur Vorschau | Bald verfügbar |
|  [Privater Kontakt](../api-reference/beta/resources/contact.md)| Allgemein verfügbar | Bald verfügbar |
|  [Benutzer](../api-reference/beta/resources/user.md) | Nur Vorschau | Nur Vorschau |

## <a name="open-extensions"></a>Offene Erweiterungen
[Offene Erweiterungen](../api-reference/beta/resources/opentypeextension.md) (früher als Office 365-Datenerweiterungen bezeichnet) sind [offene Typen](http://www.odata.org/getting-started/advanced-tutorial/#openType), die eine flexible Möglichkeit zum direkten Hinzufügen nicht typisierter App-Daten zu Ressourceninstanzen bieten. 

Offene Erweiterungen und die zugehörigen benutzerdefinierten Daten sind über die Navigationseigenschaft **extensions** der Ressourceninstanz verfügbar. Die Eigenschaft **extensionName** ist die einzige _vordefinierte_ beschreibbare Eigenschaft einer offenen Erweiterung. Bei der Erstellung einer offenen Erweiterung müssen Sie der Eigenschaft **extensionName** einen Namen zuweisen, der innerhalb des Mandanten eindeutig ist. Eine Möglichkeit hierfür ist die Verwendung eines umgekehrten DNS (Domain Name System)-Formats, das von _Ihrer eigenen Domäne_ abhängt, zum Beispiel `Com.Contoso.ContactInfo`. Verwenden Sie in Erweiterungsnamen auf keinen Fall die Microsoft-Domäne (`Com.Microsoft` oder `Com.OnMicrosoft`).

Sie können im Rahmen ein und desselben Vorgangs [eine offene Erweiterung in einer Ressourceninstanz erstellen](../api-reference/beta/api/opentypeextension_post_opentypeextension.md) und benutzerdefinierte Daten in ihr speichern. (Beachten Sie dabei die unten beschriebene [bekannte Einschränkung](#known-limitations-for-extensions) für einige der unterstützten Ressourcen.) Anschließend können Sie die Erweiterung und ihre Daten [lesen](../api-reference/beta/api/opentypeextension_get.md), [aktualisieren](../api-reference/beta/api/opentypeextension_update.md) und [löschen](../api-reference/beta/api/opentypeextension_delete.md). 

>**Hinweis:** Offene Erweiterungen sind bereits seit einiger Zeit allgemein verfügbar für Ereignisse, Gruppenbeiträge, Nachrichten und private Kontakte. Jetzt sind sie als Preview auch für administrative Einheiten, Geräte, Gruppen, Organisationen und Benutzer verfügbar.

Beispiel für eine offene Erweiterung: [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](extensibility_open_users.md)

## <a name="schema-extensions-preview"></a>Schemaerweiterungen (Preview)
Mithilfe von [Schemaerweiterungen](../api-reference/beta/resources/schemaextension.md) können Sie ein Schema definieren, das einen Ressourcentyp erweitert. Zunächst erstellen Sie eine Schemaerweiterungsdefinition. Diese verwenden Sie dann, um Ressourceninstanzen um stark typisierte benutzerdefinierte Daten zu erweitern. Sie können auch den [Status](#schema-extensions-lifecycle) Ihrer Schemaerweiterung steuern und sie so für andere Apps erkennbar machen. Die Apps können die Erweiterung dann auf ihre eigenen Daten anwenden und auf ihrer Grundlage weitere Funktionen implementieren.

Beim Erstellen einer Schemaerweiterungsdefinition müssen Sie einen eindeutigen Namen für die **ID** angeben. Es stehen zwei Benennungsoptionen zur Verfügung:

- Wenn Sie bereits über eine Vanity-`.com`-Domäne verfügen, die Sie für Ihren Mandanten überprüft haben, können Sie den Domänennamen zusammen mit dem Schemanamen verwenden, um einen eindeutigen Namen im folgenden Format zu definieren: \{_&#65279;Domänenname_\}\_\{_&#65279;Schemaname_\}. Wenn Ihre Vanity-Domäne beispielsweise „contoso.com“ ist, können Sie eine **ID** mit dem Wert `contoso_mySchema` definieren.  Dies ist die bevorzugte Option.
- Wenn Sie nicht über eine überprüfte Vanity-Domäne verfügen, können Sie die **ID** einfach auf einen Schemanamen festlegen (ohne Domänennamenpräfix), z. B. `mySchema`. Microsoft Graph weist eine Zeichenfolgen-ID anhand des angegebenen Namens im folgenden Format zu: ext\{_&#65279;8-zufällige-alphanumerische-Zeichen_\}\_\{_&#65279;Schemaname_\}.  Beispiel: `extkvbmkofy_mySchema`.

Sie sehen diesen eindeutigen Namen in der **ID**, wo er als Name des komplexen Typs verwendet wird, der Ihre benutzerdefinierten Daten in der erweiterten Ressourceninstanz speichert. 


Anders als bei offenen Erweiterungen handelt es sich bei der Verwaltung von Schemaerweiterungsdefinitionen ([Auflisten](../api-reference/beta/api/schemaextension_list.md), [Erstellen](../api-reference/beta/api/schemaextension_post_schemaextensions.md), [Abrufen](../api-reference/beta/api/schemaextension_get.md), [Aktualisieren](../api-reference/beta/api/schemaextension_update.md) und [Löschen](../api-reference/beta/api/schemaextension_delete.md)) und der Verwaltung ihrer Daten (Hinzufügen, Abrufen, Aktualisieren und Löschen) um unterschiedliche Sätze von API-Vorgängen. 

Da Schemaerweiterungen als komplexe Typen in Instanzen der Zielressourcen verfügbar sind, können Sie wie folgt CRUD-Vorgänge auf die Daten in einer Schemaerweiterung anwenden:

- Sie können die `POST`-Methode der Ressource verwenden, um bei der Erstellung einer neuen Ressourceninstanz benutzerdefinierte Daten anzugeben.
- Sie können die `GET`-Methode der Ressource verwenden, um die benutzerdefinierten Daten zu lesen.
- Sie können die `PATCH`-Methode der Ressource verwenden, um einer vorhandenen Ressourceninstanz benutzerdefinierte Daten hinzuzufügen oder benutzerdefinierte Daten aus einer vorhandenen Ressourceninstanz zu löschen.
- Sie können die `PATCH`-Methode der Ressource verwenden, um den komplexen Typ auf „null“ festzulegen und so die benutzerdefinierten Daten in der Ressourceninstanz zu löschen. 

Beispiel für eine Schemaerweiterung: [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](extensibility_schema_groups.md)


### <a name="schema-extensions-lifecycle"></a>Lebenszyklus von Schemaerweiterungen
Wenn Ihre App eine Schemaerweiterungsdefinition erstellt, wird sie als Besitzer dieser Schemaerweiterung markiert. 

Die Besitzer-App kann anschließend einen PATCH-Vorgang auf die Erweiterungseigenschaft **status** anwenden, um die Erweiterung auf den jeweils gewünschten Lebenszyklusstatus zu setzen. Je nach dem aktuellen Status kann die Besitzer-App die Erweiterung möglicherweise aktualisieren oder löschen. Jegliche Aktualisierungen einer Schemaerweiterung sollten stets ausschließlich additiv und nicht destruktiv sein.


| Status | Verhalten des Lebenszyklusstatus |
|-------------|------------|
| InDevelopment | – Anfangszustand nach der Erstellung. Die Besitzer-App entwickelt die Schemaerweiterung noch. <br> – In diesem Status kann die Schemaerweiterung nur von der Besitzer-App verwendet werden. Die Besitzer-App kann die Erweiterungsdefinition mit additiven Änderungen aktualisieren oder sie löschen. Nur die Besitzer-App kann Ressourceninstanzen mit dieser Schemadefinition erweitern, und das nur in dem Verzeichnis, in dem die Besitzer-App registriert ist. <br> – Die Besitzer-App kann die Erweiterung vom Status `InDevelopment` auf den Status `Available` setzen. |
| Available | – Die Schemaerweiterung kann von allen Apps in jedem beliebigen Mandanten verwendet werden. <br> – Sobald die Besitzer-App die Erweiterung auf `Available` setzt, kann jede App Instanzen der in der Erweiterung angegebenen Ressourcentypen benutzerdefinierte Daten hinzufügen (vorausgesetzt, die App ist zum Zugriff auf die betreffende Ressource berechtigt). Die App kann benutzerdefinierte Daten bei der Erstellung einer neuen Instanz oder bei der Aktualisierung einer bereits vorhandenen Instanz zuweisen. Nur die Besitzer-App kann die Erweiterungsdefinition mit additiven Änderungen aktualisieren oder die Erweiterung löschen. <br> – Die Besitzer-App kann die Schemaerweiterung auch vom Status `Available` auf den Status `Deprecated` setzen. |
| Deprecated | – Die Schemaerweiterungsdefinition kann nicht mehr gelesen und auch nicht mehr geändert werden. <br> – Die Erweiterung kann von keiner App angezeigt, aktualisiert, um neue Eigenschaften ergänzt oder gelöscht werden. Apps können die _Eigenschaftswerte_ der Erweiterung jedoch weiterhin lesen, aktualisieren oder löschen. <br> – Die Besitzer-App kann die Schemaerweiterung vom Status `Deprecated` auf den Status `Available` setzen. |

>**Hinweis:** Benutzerdefinierte Daten in Schemaerweiterungen mit dem Status `Deprecated` können weiterhin abgerufen und gelöscht werden. Es gibt jedoch aktuell ein [bekanntes Problem](#known-limitations-for-extensions), aufgrund dessen der Zugriff auf benutzerdefinierte Daten nicht mehr möglich ist, sobald die zugehörige Schemaerweiterung gelöscht wurde.

### <a name="supported-property-data-types"></a>Unterstützte Datentypen für Eigenschaften 
Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:

| Eigenschaftentyp | Bemerkungen |
|-------------|------------|
| Binär | Maximal 256 Bytes. |
| Boolescher Wert | Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| DateTime | Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert. |
| Ganze Zahl | 32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| Zeichenfolge | Maximal 256 Zeichen. |

>**Hinweis:** Eigenschaften mit mehreren Werten werden derzeit nicht unterstützt.

### <a name="azure-ad-directory-schema-extensions"></a>Azure AD-Verzeichnisschemaerweiterungen
Azure AD unterstützt einen ähnlichen Erweiterungstyp namens [Verzeichnisschemaerweiterung](https://msdn.microsoft.com/en-us/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions) für einige [directoryObject](../api-reference/beta/resources/directoryObject.md)-Ressourcen. Zur Erstellung und Verwaltung der Definitionen von Verzeichnisschemaerweiterungen müssen Sie die Azure AD Graph-API verwenden. Das Hinzufügen, Abrufen, Aktualisieren und Löschen von _Daten_ in den Eigenschaften dieser Erweiterungen ist jedoch auch über die Microsoft Graph-API möglich.

## <a name="permissions"></a>Berechtigungen
Um Erweiterungsdaten aus einer Ressource auslesen oder in eine Ressource schreiben zu können, benötigen Sie dieselben [Berechtigungen](../authorization/permission_scopes.md) wie zum Lesen der Ressource und zum Schreiben in die Ressource.  Damit eine App beispielsweise das Profil des angemeldeten Benutzers mit benutzerdefinierten App-Daten aktualisieren kann, muss sie die Berechtigung *User.ReadWrite.All* besitzen.

Zusätzlich muss einer App die Berechtigung *Directory.AccessAsUser.All* gewährt werden, um Schemaerweiterungsdefinitionen zu erstellen und zu verwalten.
 
## <a name="known-limitations-for-extensions"></a>Bekannte Einschränkungen für Erweiterungen
-   Wenn Sie eine Instanz von Ressourcen des Typs **administrativeUnit**, **device**, **group**, **organization** oder **user** erstellen, können Sie nicht gleichzeitig eine offene Erweiterung angeben. Sie müssen zuerst die Instanz erstellen und dann eine ``POST``-Anforderung auf diese Instanz anwenden, in der Sie die Daten der offenen Erweiterung angeben.  
-   Die Änderungsnachverfolgung (Delta-Abfrage) wird für Eigenschaften von offenen Erweiterungen oder Schemaerweiterungen nicht unterstützt.
-   Das Filtern nach Eigenschaftswerten von Schemaerweiterungen wird noch nicht unterstützt. (Unterstützung hierfür wird jedoch in Kürze implementiert).
-   Wird eine Schemaerweiterungsdefinition gelöscht, ist kein Zugriff mehr auf benutzerdefinierte Daten möglich, die auf dem gelöschten Schema basieren. Dies ist eine temporäre Einschränkung.
-   Derzeit lassen sich Schemaerweiterungen unabhängig von ihrem Status löschen. Künftig können nur Schemaerweiterungen im Status `InDevelopment` gelöscht werden.
-   Um einen komplexen Typ einer Schemaerweiterung aus einer Ressourceninstanz zu entfernen, müssen Sie alle Eigenschaftswerte des komplexen Typs auf `null` setzen.  Künftig wird es genügen, einfach den komplexen Typ der Schemaerweiterung auf `null` zu setzen.
-   Für Verzeichnisressourcen wie Benutzer, Gruppen und Geräte gilt aktuell: Für eine Ressource dürfen maximal 100 Eigenschaftswerte von Schemaerweiterungen festgelegt werden.

## <a name="extension-examples"></a>Erweiterungsbeispiele
[Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](extensibility_open_users.md)

[Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](extensibility_schema_groups.md)

## <a name="see-also"></a>Siehe auch

[Office 365-Domänen](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[Hinzufügen und Überprüfen einer Domäne für einen Office 365-Mandanten](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
