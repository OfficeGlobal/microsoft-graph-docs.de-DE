# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="f2476-101">Übersicht über die OneDrive-Dateispeicher-API</span><span class="sxs-lookup"><span data-stu-id="f2476-101">OneDrive file storage API overview</span></span>

<span data-ttu-id="f2476-102">OneDrive ist der Dateien-Hub in Office 365.</span><span class="sxs-lookup"><span data-stu-id="f2476-102">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="f2476-103">Benutzern verwenden in vielen verschiedenen Zusammenhängen Dateien, wie z. B. Microsoft Teams, Gruppen, SharePoint und mehr.</span><span class="sxs-lookup"><span data-stu-id="f2476-103">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="f2476-104">Mit OneDrive können Benutzer unabhängig davon, wo sie gespeichert werden, auf diese Dateien zugreifen. Mit Microsoft Graph können Sie eine einzelne API verwenden, um mit den Dateien zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="f2476-104">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="f2476-105">Dateien werden in Office 365 auf [Laufwerken][Drive API] gespeichert.</span><span class="sxs-lookup"><span data-stu-id="f2476-105">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="f2476-106">Benutzer können Dateien auf einem persönlichen Laufwerk – ihrem OneDrive – oder auf einem gemeinsam genutzten Laufwerk speichern, das von einer [SharePoint][]-Dokumentbibliothek betrieben wird.</span><span class="sxs-lookup"><span data-stu-id="f2476-106">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="f2476-107">Die Flexibilität von OneDrive ermöglicht Benutzern die Methode der Zusammenarbeit, die für sie am besten geeignet ist.</span><span class="sxs-lookup"><span data-stu-id="f2476-107">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="f2476-108">Benutzer können Links zu Dateien teilen, Dateien in Teamlaufwerke kopieren oder dorthin verschieben oder sogar OneDrive-Dateien an E-Mail-Nachrichten in Outlook anfügen.</span><span class="sxs-lookup"><span data-stu-id="f2476-108">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="f2476-109">Vorteile der Integration des OneDrive-Dateispeichers in der Cloud</span><span class="sxs-lookup"><span data-stu-id="f2476-109">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="f2476-110">Nutzen Sie das „Ökosystem“ mit Milliarden von Dateien.</span><span class="sxs-lookup"><span data-stu-id="f2476-110">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="f2476-111">Benutzer von OneDrive können von jedem Gerät, online oder offline, auf ihre Dateien zugreifen und Dateien mit Personen innerhalb oder außerhalb ihres Unternehmens teilen.</span><span class="sxs-lookup"><span data-stu-id="f2476-111">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="f2476-112">OneDrive ermöglicht das gemeinsame Arbeiten an Dateien in Echtzeit und in vertrauten Anwendungen wie Word, Excel und PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="f2476-112">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="f2476-113">Dateien werden mit Microsoft Graph durch anspruchsvolle Miniaturansichten für hunderte von Formaten, durch Videostreaming, Analysefunktionen und vieles mehr bereichert.</span><span class="sxs-lookup"><span data-stu-id="f2476-113">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="f2476-114">Die Daten in OneDrive sind durch erweiterte Funktionen für Sicherheit, Compliance und Verschlüsselung geschützt, denen Kunden vertrauen.</span><span class="sxs-lookup"><span data-stu-id="f2476-114">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="f2476-115">Die OneDrive-App wird auf mehr als 500 Millionen Geräten verwendet, und mehr als 85 % der Fortune 500-Unternehmen nutzen OneDrive for Business. Indem Sie Ihre App mit OneDrive integrieren, können Sie sich mit Millionen von Kunden, Lernenden und Geschäftsanwendern verbinden und dort mit Kunden interagieren, wo sie bereits den Großteil ihrer täglichen Arbeit erledigen.</span><span class="sxs-lookup"><span data-stu-id="f2476-115">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="f2476-116">Speichern Ihrer App-Dateien in einer leistungsfähigen Cloud</span><span class="sxs-lookup"><span data-stu-id="f2476-116">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="f2476-117">Wenn Sie Ihre Dateien in OneDrive speichern, kann Ihre App die Funktionen der Microsoft-Cloud nutzen, und Ihre Benutzer von jedem beliebigen Ort aus auf ihre Dateien zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f2476-117">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="f2476-118">Verwenden Sie das SDK für die [Dateiauswahl][], um in OneDrive gespeicherte Dateien in Ihrer eigenen App schnell zu öffnen, herunterzuladen, zu speichern oder zu teilen. Nutzen Sie hierbei die gleiche Oberfläche, die Benutzern von OneDrive bereits vertraut ist.</span><span class="sxs-lookup"><span data-stu-id="f2476-118">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="f2476-119">Erhalten Sie Informationen zu ausgewählten Dateien direkt vom Auswahl-SDK, oder verwenden Sie direkt die Microsoft Graph-APIs, um die Verwendung der Dateien noch weiter zu optimieren.</span><span class="sxs-lookup"><span data-stu-id="f2476-119">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="f2476-120">Verwenden Sie [spezielle Ordner][] zum Speichern von Dateien an bekannten Speicherorten in OneDrive, z. B. `Documents` und `Camera Roll`, oder weisen Sie Ihrer App einen eigenen persönlichen Ordner zu.</span><span class="sxs-lookup"><span data-stu-id="f2476-120">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="f2476-121">Direktes Bereitstellen Ihrer App für Benutzer in OneDrive</span><span class="sxs-lookup"><span data-stu-id="f2476-121">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="f2476-122">OneDrive-Kunden können Ihre App direkt in OneDrive starten oder verwenden, um Dateien zu öffnen, zu bearbeiten oder eine Vorschau anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f2476-122">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="f2476-123">Verwenden Sie die OneDrive-[Dateihandler][]-Erweiterungen, um Symbole und Vorschauen für Ihre eigenen Dateierweiterungen bereitzustellen, fügen Sie Ihre App der Schaltfläche **Neu** hinzu, oder fügen Sie der Menüleiste sogar eigene Aktionen hinzu, um Ihre App zu starten.</span><span class="sxs-lookup"><span data-stu-id="f2476-123">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="f2476-124">Arbeiten mit Inhalten in Formaten, die Ihre App umsetzen kann</span><span class="sxs-lookup"><span data-stu-id="f2476-124">Work with content in formats your app understands</span></span>

<span data-ttu-id="f2476-125">Ihre App kann Dateiinhalte in dem Format abrufen, das für Sie am praktischsten ist.</span><span class="sxs-lookup"><span data-stu-id="f2476-125">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="f2476-126">Ihre App kann [Miniaturansichten][] in einer angepassten Größe für Hunderte von verschiedenen Dateiformaten darstellen.</span><span class="sxs-lookup"><span data-stu-id="f2476-126">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="f2476-127">Sie können Dateien in einer Vielzahl von alternativen [Formaten][] herunterladen, wie z. B. PDF.</span><span class="sxs-lookup"><span data-stu-id="f2476-127">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="f2476-128">Sie können die Vorschauprogramme für OneDrive-Dateien in Ihre App einbetten, indem Sie die [Vorschau][]-API (Beta) verwenden.</span><span class="sxs-lookup"><span data-stu-id="f2476-128">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="f2476-129">Arbeiten mit Dateiinhalten und Metadaten ohne Herunterladen der Binary</span><span class="sxs-lookup"><span data-stu-id="f2476-129">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="f2476-130">Mit Microsoft Graph können Sie über die REST-APIs auf komplexe Inhalte zugreifen, ohne die Binary herunterladen zu müssen.</span><span class="sxs-lookup"><span data-stu-id="f2476-130">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="f2476-131">Sehen Sie sich die aus [Bild][]-, [Audio][]- und [Video][]-Dateien extrahierten Metadaten an.</span><span class="sxs-lookup"><span data-stu-id="f2476-131">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="f2476-132">Verwenden Sie die [Excel-API][], um die in einer Excel-Arbeitsmappe gespeicherten Rohdaten direkt zu bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="f2476-132">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="f2476-133">Verwenden Sie die [Notizen-API][] zum Zugreifen auf Inhalte in OneNote-Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="f2476-133">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="f2476-134">Reagieren auf Dateiänderungen</span><span class="sxs-lookup"><span data-stu-id="f2476-134">React to file changes</span></span>

<span data-ttu-id="f2476-135">Ihre App kann anhand von [Webhooks][] benachrichtigt werden, wenn sich Dateien ändern, damit Sie schnell reagieren können.</span><span class="sxs-lookup"><span data-stu-id="f2476-135">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="f2476-136">Verwenden Sie die [Delta-API-][], um die Änderungen seit der letzten Synchronisierung Ihrer App mit der Cloud anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f2476-136">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f2476-137">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f2476-137">Next steps</span></span>

<span data-ttu-id="f2476-138">Erfahren Sie mehr über das [Verwenden der OneDrive-API] [ Drive API] in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="f2476-138">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[Dateiauswahl]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[File picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[Dateihandler]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
<span data-ttu-id="f2476-142">
  [Spezielle Ordner]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span><span class="sxs-lookup"><span data-stu-id="f2476-142">[Special folders]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span></span>
<span data-ttu-id="f2476-143">
  [Notizen-API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span><span class="sxs-lookup"><span data-stu-id="f2476-143">[Notes API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span></span>
<span data-ttu-id="f2476-144">
  [Excel-API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span><span class="sxs-lookup"><span data-stu-id="f2476-144">[Excel API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span></span>
[REST API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
<span data-ttu-id="f2476-145">
  [Delta-API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span><span class="sxs-lookup"><span data-stu-id="f2476-145">[delta API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span></span>
<span data-ttu-id="f2476-146">
  [Video]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span><span class="sxs-lookup"><span data-stu-id="f2476-146">[video]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span></span>
<span data-ttu-id="f2476-147">
  [Foto]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span><span class="sxs-lookup"><span data-stu-id="f2476-147">[photo]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span></span>
<span data-ttu-id="f2476-148">
  [Audio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span><span class="sxs-lookup"><span data-stu-id="f2476-148">[audio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span></span>
<span data-ttu-id="f2476-149">
  [Formate]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span><span class="sxs-lookup"><span data-stu-id="f2476-149">[Formats]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span></span>
<span data-ttu-id="f2476-150">
  [Miniaturansichten]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span><span class="sxs-lookup"><span data-stu-id="f2476-150">[thumbnails]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span></span>
<span data-ttu-id="f2476-151">
  [Vorschau]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span><span class="sxs-lookup"><span data-stu-id="f2476-151">[Preview]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span></span>
<span data-ttu-id="f2476-152">
  [Webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span><span class="sxs-lookup"><span data-stu-id="f2476-152">[Webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span></span>
[Drive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
