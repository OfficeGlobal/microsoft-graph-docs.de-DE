# <a name="onedrive-file-storage-api-overview"></a>Übersicht über die OneDrive-Dateispeicher-API

OneDrive ist der Dateien-Hub in Office 365.
Benutzern verwenden in vielen verschiedenen Zusammenhängen Dateien, wie z. B. Microsoft Teams, Gruppen, SharePoint und mehr.
Mit OneDrive können Benutzer unabhängig davon, wo sie gespeichert werden, auf diese Dateien zugreifen. Mit Microsoft Graph können Sie eine einzelne API verwenden, um mit den Dateien zu arbeiten.

Dateien werden in Office 365 auf [Laufwerken][Drive API] gespeichert.
Benutzer können Dateien auf einem persönlichen Laufwerk – ihrem OneDrive – oder auf einem gemeinsam genutzten Laufwerk speichern, das von einer [SharePoint][]-Dokumentbibliothek betrieben wird.
Die Flexibilität von OneDrive ermöglicht Benutzern die Methode der Zusammenarbeit, die für sie am besten geeignet ist.
Benutzer können Links zu Dateien teilen, Dateien in Teamlaufwerke kopieren oder dorthin verschieben oder sogar OneDrive-Dateien an E-Mail-Nachrichten in Outlook anfügen.

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a>Vorteile der Integration des OneDrive-Dateispeichers in der Cloud

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a>Nutzen Sie das „Ökosystem“ mit Milliarden von Dateien.

Benutzer von OneDrive können von jedem Gerät, online oder offline, auf ihre Dateien zugreifen und Dateien mit Personen innerhalb oder außerhalb ihres Unternehmens teilen.
OneDrive ermöglicht das gemeinsame Arbeiten an Dateien in Echtzeit und in vertrauten Anwendungen wie Word, Excel und PowerPoint.
Dateien werden mit Microsoft Graph durch anspruchsvolle Miniaturansichten für hunderte von Formaten, durch Videostreaming, Analysefunktionen und vieles mehr bereichert.
Die Daten in OneDrive sind durch erweiterte Funktionen für Sicherheit, Compliance und Verschlüsselung geschützt, denen Kunden vertrauen.

Die OneDrive-App wird auf mehr als 500 Millionen Geräten verwendet, und mehr als 85 % der Fortune 500-Unternehmen nutzen OneDrive for Business. Indem Sie Ihre App mit OneDrive integrieren, können Sie sich mit Millionen von Kunden, Lernenden und Geschäftsanwendern verbinden und dort mit Kunden interagieren, wo sie bereits den Großteil ihrer täglichen Arbeit erledigen.

### <a name="store-your-apps-files-in-a-powerful-cloud"></a>Speichern Ihrer App-Dateien in einer leistungsfähigen Cloud

Wenn Sie Ihre Dateien in OneDrive speichern, kann Ihre App die Funktionen der Microsoft-Cloud nutzen, und Ihre Benutzer von jedem beliebigen Ort aus auf ihre Dateien zugreifen.
Verwenden Sie das SDK für die [Dateiauswahl][], um in OneDrive gespeicherte Dateien in Ihrer eigenen App schnell zu öffnen, herunterzuladen, zu speichern oder zu teilen. Nutzen Sie hierbei die gleiche Oberfläche, die Benutzern von OneDrive bereits vertraut ist.
Erhalten Sie Informationen zu ausgewählten Dateien direkt vom Auswahl-SDK, oder verwenden Sie direkt die Microsoft Graph-APIs, um die Verwendung der Dateien noch weiter zu optimieren.
Verwenden Sie [spezielle Ordner][] zum Speichern von Dateien an bekannten Speicherorten in OneDrive, z. B. `Documents` und `Camera Roll`, oder weisen Sie Ihrer App einen eigenen persönlichen Ordner zu.

### <a name="bring-your-app-straight-to-users-within-onedrive"></a>Direktes Bereitstellen Ihrer App für Benutzer in OneDrive

OneDrive-Kunden können Ihre App direkt in OneDrive starten oder verwenden, um Dateien zu öffnen, zu bearbeiten oder eine Vorschau anzuzeigen.
Verwenden Sie die OneDrive-[Dateihandler][]-Erweiterungen, um Symbole und Vorschauen für Ihre eigenen Dateierweiterungen bereitzustellen, fügen Sie Ihre App der Schaltfläche **Neu** hinzu, oder fügen Sie der Menüleiste sogar eigene Aktionen hinzu, um Ihre App zu starten.

### <a name="work-with-content-in-formats-your-app-understands"></a>Arbeiten mit Inhalten in Formaten, die Ihre App umsetzen kann

Ihre App kann Dateiinhalte in dem Format abrufen, das für Sie am praktischsten ist.
Ihre App kann [Miniaturansichten][] in einer angepassten Größe für Hunderte von verschiedenen Dateiformaten darstellen.
Sie können Dateien in einer Vielzahl von alternativen [Formaten][] herunterladen, wie z. B. PDF.
Sie können die Vorschauprogramme für OneDrive-Dateien in Ihre App einbetten, indem Sie die [Vorschau][]-API (Beta) verwenden.

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a>Arbeiten mit Dateiinhalten und Metadaten ohne Herunterladen der Binary

Mit Microsoft Graph können Sie über die REST-APIs auf komplexe Inhalte zugreifen, ohne die Binary herunterladen zu müssen.
Sehen Sie sich die aus [Bild][]-, [Audio][]- und [Video][]-Dateien extrahierten Metadaten an.
Verwenden Sie die [Excel-API][], um die in einer Excel-Arbeitsmappe gespeicherten Rohdaten direkt zu bearbeiten.
Verwenden Sie die [Notizen-API][] zum Zugreifen auf Inhalte in OneNote-Notizbüchern.

### <a name="react-to-file-changes"></a>Reagieren auf Dateiänderungen

Ihre App kann anhand von [Webhooks][] benachrichtigt werden, wenn sich Dateien ändern, damit Sie schnell reagieren können.
Verwenden Sie die [Delta-API-][], um die Änderungen seit der letzten Synchronisierung Ihrer App mit der Cloud anzuzeigen.

## <a name="next-steps"></a>Nächste Schritte

Erfahren Sie mehr über das [Verwenden der OneDrive-API] [ Drive API] in Microsoft Graph v1.0.

[SharePoint]: sharepoint-concept-overview.md
[Dateiauswahl]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[Dateihandler]: https://docs.microsoft.com/onedrive/developer/file-handlers

  [Spezielle Ordner]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder

  [Notizen-API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote

  [Excel-API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel
[REST API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive

  [Delta-API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta

  [Video]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video

  [Foto]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo

  [Audio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio

  [Formate]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format

  [Miniaturansichten]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails

  [Vorschau]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview

  [Webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks
[Drive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
