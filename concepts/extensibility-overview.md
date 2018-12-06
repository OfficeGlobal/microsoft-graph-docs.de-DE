---
title: Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen
description: Microsoft Graph stellt einen zentralen API-Endpunkt bereit, der Ihnen über verschiedene Ressourcen wie user und message Zugriff auf umfassende personenzentrierte Daten und Erkenntnisse ermöglicht. Sie können auch Microsoft Graph um eigene Anwendungsdaten erweitern. Sie können Microsoft Graph-Ressourcen benutzerdefinierte Eigenschaften hinzufügen, ohne dass dafür ein externer Datenspeicher nötig wäre.
ms.openlocfilehash: f63ce3a9b7751452427bc79443c3a0186a8d3ca9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092193"
---
# <a name="add-custom-data-to-resources-using-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen

Microsoft Graph stellt einen zentralen API-Endpunkt bereit, der Ihnen über verschiedene Ressourcen wie [user](/graph/api/resources/user?view=graph-rest-1.0) und [message](/graph/api/resources/message?view=graph-rest-1.0) Zugriff auf umfassende personenzentrierte Daten und Erkenntnisse ermöglicht. Sie können auch Microsoft Graph um eigene Anwendungsdaten erweitern. Sie können Microsoft Graph-Ressourcen benutzerdefinierte Eigenschaften hinzufügen, ohne dass dafür ein externer Datenspeicher nötig wäre.

So könnten Sie sich beispielsweise entscheiden, Ihre App schlank zu halten und App-spezifische Benutzerprofildaten in Microsoft Graph zu speichern, indem Sie die Ressource **user** erweitern. Alternativ könnten Sie den vorhandenen Benutzerprofilspeicher Ihrer App auch beibehalten und der Ressource **user** einfach einen App-spezifischen Speicherbezeichner hinzufügen.

Microsoft Graph bietet zwei Arten von Erweiterungen. Wählen Sie den Erweiterungstyp aus, der Ihren Anwendungsanforderungen am besten entspricht:

- **Offene Erweiterungen**: Dieser Erweiterungstyp ist ideal für die ersten Schritte mit Erweiterungen.
- **Schemaerweiterungen**: Bei diesem Erweiterungstyp handelt es sich um einen flexibleren Mechanismus für Entwickler, die typisierte Daten speichern, ihr Schema erkennbar und gemeinsam nutzbar machen, Filteroptionen nutzen und später auch Autorisierung und die Überprüfung von Eingabedaten implementieren möchten.

> **Wichtig:** Sie sollten Erweiterungen nicht zur Speicherung vertraulicher personenbezogener Informationen wie Kontoanmeldeinformationen, Behördenkennnummern, Karteninhaberdaten, Bankkontonummern, Krankendaten oder vertraulichen Hintergrundinformationen verwenden.

## <a name="supported-resources"></a>Unterstützte Ressourcen

In der folgenden Tabelle sind die Ressourcen aufgeführt, die offene Erweiterungen und Schemaerweiterungen unterstützen und angeben, ob sie die allgemeine Verfügbarkeit (GA) erreicht haben (verfügbar sowohl in v1.0- und Beta-Endpunkten) oder sich in der Vorschau befinden (nur im Beta-Endpunkt verfügbar).

|Ressource |Offene Erweiterungen |Schemaerweiterungen |
|:------- |:------ |:------ |
| [Administrative Einheit](/graph/api/resources/administrativeunit?view=graph-rest-beta) | Nur Vorschau | Nur Vorschau |
| [Kalenderereignis](/graph/api/resources/event?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Gerät](/graph/api/resources/device?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Gruppe](/graph/api/resources/group?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Kalenderereignis für Gruppe](/graph/api/resources/event?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Beitrag zu Gruppenunterhaltung](/graph/api/resources/post?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Nachricht](/graph/api/resources/message?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Organisation](/graph/api/resources/organization?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |
| [Privater Kontakt](/graph/api/resources/contact?view=graph-rest-1.0)| Allgemein verfügbar | Allgemein verfügbar |
| [Benutzer](/graph/api/resources/user?view=graph-rest-1.0) | Allgemein verfügbar | Allgemein verfügbar |

Sie können Erweiterungen für alle diese Ressourcen verwenden, wenn Sie mit einem Geschäfts-, Schul- oder Unikonto angemeldet sind. Darüber hinaus können Sie Erweiterungen für die folgenden Ressourcen verwenden, wenn Sie mit einem persönlichen Konto angemeldet sind: **event**, **post**, **group**, **message**, **contact** und **user**.

## <a name="open-extensions"></a>Offene Erweiterungen

[Offene Erweiterungen](/graph/api/resources/opentypeextension?view=graph-rest-1.0) (früher als Office 365-Datenerweiterungen bezeichnet) sind [offene Typen](https://www.odata.org/getting-started/advanced-tutorial/#openType), die eine flexible Möglichkeit zum direkten Hinzufügen nicht typisierter App-Daten zu Ressourceninstanzen bieten.

Offene Erweiterungen und die zugehörigen benutzerdefinierten Daten sind über die Navigationseigenschaft **extensions** der Ressourceninstanz verfügbar.
Die Eigenschaft **extensionName** ist die einzige _vordefinierte_ beschreibbare Eigenschaft einer offenen Erweiterung. Bei der Erstellung einer offenen Erweiterung müssen Sie der Eigenschaft **extensionName** einen Namen zuweisen, der innerhalb des Mandanten eindeutig ist.

Eine Möglichkeit hierfür ist die Verwendung eines umgekehrten DNS (Domain Name System)-Formats, das von _Ihrer eigenen Domäne_ abhängt, zum Beispiel `Com.Contoso.ContactInfo`.

Verwenden Sie in Erweiterungsnamen auf keinen Fall die Microsoft-Domäne (`Com.Microsoft` oder `Com.OnMicrosoft`).

Sie können im Rahmen ein und desselben Vorgangs [eine offene Erweiterung in einer Ressourceninstanz erstellen](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0) und benutzerdefinierte Daten in ihr speichern. (Beachten Sie dabei die [bekannte Einschränkung](known-issues.md#extensions) für einige der unterstützten Ressourcen.)

Anschließend können Sie die Erweiterung und ihre Daten [lesen](/graph/api/opentypeextension-get?view=graph-rest-1.0), [aktualisieren](/graph/api/opentypeextension-update?view=graph-rest-1.0) und [löschen](/graph/api/opentypeextension-delete?view=graph-rest-1.0).

Beispiel für eine offene Erweiterung: [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](extensibility-open-users.md)

## <a name="schema-extensions"></a>Schemaerweiterungen

Mithilfe von [Schemaerweiterungen](/graph/api/resources/schemaextension?view=graph-rest-1.0) können Sie ein Schema definieren, das einen Ressourcentyp erweitert. Zunächst erstellen Sie eine Schemaerweiterungsdefinition. Diese verwenden Sie dann, um Ressourceninstanzen um stark typisierte benutzerdefinierte Daten zu erweitern. Sie können auch den [Status](#schema-extensions-lifecycle) Ihrer Schemaerweiterung steuern und sie so für andere Apps erkennbar machen. Die Apps können die Erweiterung dann auf ihre eigenen Daten anwenden und auf ihrer Grundlage weitere Funktionen implementieren.

Beim Erstellen einer Schemaerweiterungsdefinition müssen Sie einen eindeutigen Namen für die **ID** angeben. Es stehen zwei Benennungsoptionen zur Verfügung:

- Wenn Sie bereits über eine Vanity-`.com`-, `.net`-,  `.gov`-, `.edu`- oder `.org`-Domäne verfügen, die Sie für Ihren Mandanten überprüft haben, können Sie den Domänennamen zusammen mit dem Schemanamen verwenden, um einen eindeutigen Namen im folgenden Format zu definieren: \{_&#65279;Domänenname_\}\_\{_&#65279;Schemaname_\}. Wenn Ihre Vanity-Domäne beispielsweise „contoso.com“ ist, können Sie eine **ID** mit dem Wert `contoso_mySchema` definieren. Dies ist die bevorzugte Option.
- Wenn Sie nicht über eine überprüfte Vanity-Domäne verfügen, können Sie die **ID** einfach auf einen Schemanamen festlegen (ohne Domänennamenpräfix), z. B. `mySchema`. Microsoft Graph weist eine Zeichenfolgen-ID anhand des angegebenen Namens im folgenden Format zu: ext\{_&#65279;8-zufällige-alphanumerische-Zeichen_\}\_\{_&#65279;Schemaname_\}.  Beispiel: `extkvbmkofy_mySchema`.

Sie sehen diesen eindeutigen Namen in der **ID**, wo er als Name des komplexen Typs verwendet wird, der Ihre benutzerdefinierten Daten in der erweiterten Ressourceninstanz speichert.

Anders als bei offenen Erweiterungen handelt es sich bei der Verwaltung von Schemaerweiterungsdefinitionen ([Auflisten](/graph/api/schemaextension-list?view=graph-rest-1.0), [Erstellen](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0), [Abrufen](/graph/api/schemaextension-get?view=graph-rest-1.0), [Aktualisieren](/graph/api/schemaextension-update?view=graph-rest-1.0) und [Löschen](/graph/api/schemaextension-delete?view=graph-rest-1.0)) und der Verwaltung ihrer Daten (Hinzufügen, Abrufen, Aktualisieren und Löschen) um unterschiedliche Sätze von API-Vorgängen.

Da Schemaerweiterungen als komplexe Typen in Instanzen der Zielressourcen zugänglich sind, können Sie wie folgt CRUD-Vorgänge auf die benutzerdefinierten Daten in einer Schemaerweiterung anwenden:

- Sie können die `POST`-Methode der Ressource verwenden, um bei der Erstellung einer neuen Ressourceninstanz benutzerdefinierte Daten anzugeben. Beachten Sie, dass ein [bekanntes Problem](known-issues.md#creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time) für die Ressourcen **contact**, **event**, **message** und **post** vorhanden ist, für das Sie eine Schemaerweiterung über einen `PATCH`-Vorgang erstellen müssen.
- Sie können die `GET`-Methode der Ressource verwenden, um die benutzerdefinierten Daten zu lesen.
- Sie können die `PATCH`-Methode der Ressource verwenden, um einer vorhandenen Ressourceninstanz benutzerdefinierte Daten hinzuzufügen oder benutzerdefinierte Daten aus einer vorhandenen Ressourceninstanz zu löschen.
- Sie können die `PATCH`-Methode der Ressource verwenden, um den komplexen Typ auf „null“ festzulegen und so die benutzerdefinierten Daten in der Ressourceninstanz zu löschen.

Beispiel für eine Schemaerweiterung: [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](extensibility-schema-groups.md)

### <a name="schema-extensions-lifecycle"></a>Lebenszyklus von Schemaerweiterungen

Wenn Ihre App eine Schemaerweiterungsdefinition erstellt, wird sie als Besitzer dieser Schemaerweiterung markiert.

Die Besitzer-App kann anschließend einen PATCH-Vorgang auf die Erweiterungseigenschaft **status** anwenden, um die Erweiterung auf den jeweils gewünschten Lebenszyklusstatus zu setzen. Je nach dem aktuellen Status kann die Besitzer-App die Erweiterung möglicherweise aktualisieren oder löschen. Jegliche Aktualisierungen einer Schemaerweiterung sollten stets ausschließlich additiv und nicht destruktiv sein.

|Status |Verhalten des Lebenszyklusstatus |
|:-------------|:------------|
| InDevelopment | <ul><li>Anfänglicher Status nach der Erstellung. Die Besitzer-App entwickelt die Schemaerweiterung noch. </li><li>In diesem Status kann jede App Ressourceninstanzen mit dieser Schemadefinition erweitern, und das nur in dem Verzeichnis, in dem die Besitzer-App registriert ist. </li><li>Nur die Besitzer-App kann die Erweiterungsdefinition mit additiven Änderungen aktualisieren oder sie löschen. </li><li>Die Besitzer-App kann die Schemaerweiterung aus dem Status **InDevelopment** in den Status **Available** versetzen.</li></ul> |
| Available | <ul><li>Die Schemaerweiterung kann von allen Apps in jedem beliebigen Mandanten verwendet werden. </li><li>Nachdem die Besitzer-App die Erweiterung auf **Available** festlegt, kann jede App benutzerdefinierte Daten zu Instanzen der in der Erweiterung angegebenen Ressourcentypen hinzufügen (vorausgesetzt, die App ist zum Zugriff auf die betreffende Ressource berechtigt). Die App kann benutzerdefinierte Daten bei der Erstellung einer neuen Instanz oder bei der Aktualisierung einer bereits vorhandenen Instanz zuweisen. </li><li>Nur die Besitzer-App kann die Erweiterungsdefinition mit additiven Änderungen aktualisieren. Die Erweiterungsdefinition kann in diesem Status von keiner App gelöscht werden. </li><li>Die Besitzer-App kann die Schemaerweiterung aus dem Status **Available** in den Status **Deprecated** versetzen.</li></ul> |
| Deprecated | <ul><li>Die Schemaerweiterungsdefinition kann nicht mehr gelesen und auch nicht mehr geändert werden. </li><li>Die Erweiterung kann von keiner App angezeigt, aktualisiert, um neue Eigenschaften ergänzt oder gelöscht werden. </li><li>Apps können vorhandene _Eigenschaftswerte_ der Erweiterung jedoch weiterhin lesen, aktualisieren oder löschen. </li></ul> |

### <a name="supported-property-data-types"></a>Unterstützte Datentypen für Eigenschaften

Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:

| Eigenschaftentyp | Bemerkungen |
|:-------------|:------------|
| Binär | Maximal 256 Bytes. |
| Boolescher Wert | Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| DateTime | Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert. |
| Ganze Zahl | 32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| Zeichenfolge | Maximal 256 Zeichen. |

> **Hinweis:** Eigenschaften mit mehreren Werten werden nicht unterstützt.

### <a name="azure-ad-directory-schema-extensions"></a>Azure AD-Verzeichnisschemaerweiterungen

Azure AD unterstützt einen ähnlichen Erweiterungstyp namens [Verzeichnisschemaerweiterung](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions) für einige [directoryObject-Ressourcen](/graph/api/resources/directoryobject?view=graph-rest-1.0). Zur Erstellung und Verwaltung der Definitionen von Verzeichnisschemaerweiterungen müssen Sie die [Azure AD Graph-API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) verwenden. Das Hinzufügen, Abrufen, Aktualisieren und Löschen von _Daten_ in den Eigenschaften dieser Erweiterungen ist jedoch auch über die Microsoft Graph-API möglich.

## <a name="permissions"></a>Berechtigungen

Um Erweiterungsdaten aus einer Ressource auslesen oder in eine Ressource schreiben zu können, benötigen Sie dieselben [Berechtigungen](./permissions-reference.md) wie zum Lesen der Ressource und zum Schreiben in die Ressource. Damit eine App beispielsweise das Profil des angemeldeten Benutzers mit benutzerdefinierten App-Daten aktualisieren kann, muss sie die Berechtigung *User.ReadWrite.All* besitzen.

Zusätzlich muss einer App die Berechtigung *Directory.AccessAsUser.All* gewährt werden, um Schemaerweiterungsdefinitionen zu erstellen und zu verwalten.

## <a name="data-limits"></a>Beschränkungen für Daten

### <a name="open-extension-limits"></a>Beschränkungen für offene Erweiterungen

Die folgenden Beschränkungen gelten für Verzeichnisressourcen (z. B. **user**, **group**, **device**):

- Jede offene Erweiterung kann bis zu 2 KB Daten enthalten (einschließlich der Erweiterungsdefinition selbst).
- Eine Anwendung kann bis zu zwei offene Erweiterungen pro Ressourceninstanz hinzufügen.

Die folgenden Grenzwerte gelten für Outlook-Ressourcen (z.B. **Nachricht**, **Ereignis** und **Kontakt**):

- Jede offene Erweiterung ist in einer [benannten MAPI-Eigenschaft](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx) gespeichert, die eine begrenzte Ressource in dem Postfach eines Benutzers darstellt. Weitere Informationen hierzu finden Sie unter [openTypeExtension-Ressourcentyp](/graph/api/resources/opentypeextension?view=graph-rest-1.0).

### <a name="schema-extension-limits"></a>Beschränkungen für Schemaerweiterungen

Eine Anwendung kann nicht mehr als fünf **Schemaerweiterungs**definitionen erstellen.

## <a name="known-limitations"></a>Bekannte Einschränkungen

Bekannte Einschränkungen bei der Verwendung von Erweiterungen finden Sie im [Abschnitt zu Erweiterungen](known-issues.md#extensions) im Artikel über bekannte Probleme.

## <a name="extension-examples"></a>Erweiterungsbeispiele

- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](extensibility-open-users.md)

- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](extensibility-schema-groups.md)

## <a name="see-also"></a>Siehe auch

- [Office 365-Domänen](https://technet.microsoft.com/de-DE/library/office-365-domains.aspx)

- [Hinzufügen und Überprüfen einer Domäne für einen Office 365-Mandanten](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
