---
title: Übersicht über die OneDrive-Dateispeicher-API
description: OneDrive ist der Dateien-Hub in Office 365.
ms.openlocfilehash: dcd16969a2f1b1f6898696fe0be9539d50800252
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092159"
---
# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="421a4-103">Übersicht über die OneDrive-Dateispeicher-API</span><span class="sxs-lookup"><span data-stu-id="421a4-103">OneDrive file storage API overview</span></span>

<span data-ttu-id="421a4-104">OneDrive ist der Dateien-Hub in Office 365.</span><span class="sxs-lookup"><span data-stu-id="421a4-104">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="421a4-105">Benutzern verwenden in vielen verschiedenen Zusammenhängen Dateien, wie z. B. Microsoft Teams, Gruppen, SharePoint und mehr.</span><span class="sxs-lookup"><span data-stu-id="421a4-105">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="421a4-106">Mit OneDrive können Benutzer unabhängig davon, wo sie gespeichert werden, auf diese Dateien zugreifen. Mit Microsoft Graph können Sie eine einzelne API verwenden, um mit den Dateien zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="421a4-106">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="421a4-107">Dateien werden in Office 365 auf [Laufwerken][Drive API] gespeichert.</span><span class="sxs-lookup"><span data-stu-id="421a4-107">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="421a4-108">Benutzer können Dateien auf einem persönlichen Laufwerk – ihrem OneDrive – oder auf einem gemeinsam genutzten Laufwerk speichern, das von einer [SharePoint][]-Dokumentbibliothek betrieben wird.</span><span class="sxs-lookup"><span data-stu-id="421a4-108">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="421a4-109">Die Flexibilität von OneDrive ermöglicht Benutzern die Methode der Zusammenarbeit, die für sie am besten geeignet ist.</span><span class="sxs-lookup"><span data-stu-id="421a4-109">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="421a4-110">Benutzer können Links zu Dateien teilen, Dateien in Teamlaufwerke kopieren oder dorthin verschieben oder sogar OneDrive-Dateien an E-Mail-Nachrichten in Outlook anfügen.</span><span class="sxs-lookup"><span data-stu-id="421a4-110">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="421a4-111">Vorteile der Integration des OneDrive-Dateispeichers in der Cloud</span><span class="sxs-lookup"><span data-stu-id="421a4-111">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="421a4-112">Nutzen Sie das „Ökosystem“ mit Milliarden von Dateien.</span><span class="sxs-lookup"><span data-stu-id="421a4-112">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="421a4-113">Benutzer von OneDrive können von jedem Gerät, online oder offline, auf ihre Dateien zugreifen und Dateien mit Personen innerhalb oder außerhalb ihres Unternehmens teilen.</span><span class="sxs-lookup"><span data-stu-id="421a4-113">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="421a4-114">OneDrive ermöglicht das gemeinsame Arbeiten an Dateien in Echtzeit und in vertrauten Anwendungen wie Word, Excel und PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="421a4-114">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="421a4-115">Dateien werden mit Microsoft Graph durch anspruchsvolle Miniaturansichten für hunderte von Formaten, durch Videostreaming, Analysefunktionen und vieles mehr bereichert.</span><span class="sxs-lookup"><span data-stu-id="421a4-115">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="421a4-116">Die Daten in OneDrive sind durch erweiterte Funktionen für Sicherheit, Compliance und Verschlüsselung geschützt, denen Kunden vertrauen.</span><span class="sxs-lookup"><span data-stu-id="421a4-116">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="421a4-117">Die OneDrive-App wird auf mehr als 500 Millionen Geräten verwendet, und mehr als 85 % der Fortune 500-Unternehmen nutzen OneDrive for Business. Indem Sie Ihre App mit OneDrive integrieren, können Sie sich mit Millionen von Kunden, Lernenden und Geschäftsanwendern verbinden und dort mit Kunden interagieren, wo sie bereits den Großteil ihrer täglichen Arbeit erledigen.</span><span class="sxs-lookup"><span data-stu-id="421a4-117">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="421a4-118">Speichern Ihrer App-Dateien in einer leistungsfähigen Cloud</span><span class="sxs-lookup"><span data-stu-id="421a4-118">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="421a4-119">Wenn Sie Ihre Dateien in OneDrive speichern, kann Ihre App die Funktionen der Microsoft-Cloud nutzen, und Ihre Benutzer von jedem beliebigen Ort aus auf ihre Dateien zugreifen.</span><span class="sxs-lookup"><span data-stu-id="421a4-119">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="421a4-120">Verwenden Sie das SDK für die [Dateiauswahl][], um in OneDrive gespeicherte Dateien in Ihrer eigenen App schnell zu öffnen, herunterzuladen, zu speichern oder zu teilen. Nutzen Sie hierbei die gleiche Oberfläche, die Benutzern von OneDrive bereits vertraut ist.</span><span class="sxs-lookup"><span data-stu-id="421a4-120">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="421a4-121">Erhalten Sie Informationen zu ausgewählten Dateien direkt vom Auswahl-SDK, oder verwenden Sie direkt die Microsoft Graph-APIs, um die Verwendung der Dateien noch weiter zu optimieren.</span><span class="sxs-lookup"><span data-stu-id="421a4-121">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="421a4-122">Verwenden Sie [spezielle Ordner][] zum Speichern von Dateien an bekannten Speicherorten in OneDrive, z. B. `Documents` und `Camera Roll`, oder weisen Sie Ihrer App einen eigenen persönlichen Ordner zu.</span><span class="sxs-lookup"><span data-stu-id="421a4-122">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="421a4-123">Direktes Bereitstellen Ihrer App für Benutzer in OneDrive</span><span class="sxs-lookup"><span data-stu-id="421a4-123">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="421a4-124">OneDrive-Kunden können Ihre App direkt in OneDrive starten oder verwenden, um Dateien zu öffnen, zu bearbeiten oder eine Vorschau anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="421a4-124">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="421a4-125">Verwenden Sie die OneDrive-[Dateihandler][]-Erweiterungen, um Symbole und Vorschauen für Ihre eigenen Dateierweiterungen bereitzustellen, fügen Sie Ihre App der Schaltfläche **Neu** hinzu, oder fügen Sie der Menüleiste sogar eigene Aktionen hinzu, um Ihre App zu starten.</span><span class="sxs-lookup"><span data-stu-id="421a4-125">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="421a4-126">Arbeiten mit Inhalten in Formaten, die Ihre App umsetzen kann</span><span class="sxs-lookup"><span data-stu-id="421a4-126">Work with content in formats your app understands</span></span>

<span data-ttu-id="421a4-127">Ihre App kann Dateiinhalte in dem Format abrufen, das für Sie am praktischsten ist.</span><span class="sxs-lookup"><span data-stu-id="421a4-127">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="421a4-128">Ihre App kann [Miniaturansichten][] in einer angepassten Größe für Hunderte von verschiedenen Dateiformaten darstellen.</span><span class="sxs-lookup"><span data-stu-id="421a4-128">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="421a4-129">Sie können Dateien in einer Vielzahl von alternativen [Formaten][] herunterladen, wie z. B. PDF.</span><span class="sxs-lookup"><span data-stu-id="421a4-129">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="421a4-130">Sie können die Vorschauprogramme für OneDrive-Dateien in Ihre App einbetten, indem Sie die [Vorschau][]-API (Beta) verwenden.</span><span class="sxs-lookup"><span data-stu-id="421a4-130">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="421a4-131">Arbeiten mit Dateiinhalten und Metadaten ohne Herunterladen der Binary</span><span class="sxs-lookup"><span data-stu-id="421a4-131">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="421a4-132">Mit Microsoft Graph können Sie über die REST-APIs auf komplexe Inhalte zugreifen, ohne die Binary herunterladen zu müssen.</span><span class="sxs-lookup"><span data-stu-id="421a4-132">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="421a4-133">Sehen Sie sich die aus [Bild][]-, [Audio][]- und [Video][]-Dateien extrahierten Metadaten an.</span><span class="sxs-lookup"><span data-stu-id="421a4-133">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="421a4-134">Verwenden Sie die [Excel-API][], um die in einer Excel-Arbeitsmappe gespeicherten Rohdaten direkt zu bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="421a4-134">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="421a4-135">Verwenden Sie die [Notizen-API][] zum Zugreifen auf Inhalte in OneNote-Notizbüchern.</span><span class="sxs-lookup"><span data-stu-id="421a4-135">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="421a4-136">Reagieren auf Dateiänderungen</span><span class="sxs-lookup"><span data-stu-id="421a4-136">React to file changes</span></span>

<span data-ttu-id="421a4-137">Ihre App kann anhand von [Webhooks][] benachrichtigt werden, wenn sich Dateien ändern, damit Sie schnell reagieren können.</span><span class="sxs-lookup"><span data-stu-id="421a4-137">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="421a4-138">Verwenden Sie die [Delta-API][], um die Änderungen seit der letzten Synchronisierung Ihrer App mit der Cloud anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="421a4-138">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="api-reference"></a><span data-ttu-id="421a4-139">API-Referenz</span><span class="sxs-lookup"><span data-stu-id="421a4-139">API reference</span></span>
<span data-ttu-id="421a4-140">Suchen Sie die API-Referenz für diesen Dienst?</span><span class="sxs-lookup"><span data-stu-id="421a4-140">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="421a4-141">OneDrive-Dateispeicher-API in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="421a4-141">OneDrive file storage API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onedrive?view=graph-rest-1.0)
- [<span data-ttu-id="421a4-142">OneDrive-Dateispeicher-API in Microsoft Graph, Betaversion</span><span class="sxs-lookup"><span data-stu-id="421a4-142">OneDrive file storage API in Microsoft Graph beta</span></span>](/graph/api/resources/onedrive?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="421a4-143">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="421a4-143">Next steps</span></span>

<span data-ttu-id="421a4-144">Erfahren Sie mehr über das [Verwenden der OneDrive-API] [ Drive API] in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="421a4-144">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[Dateiauswahl]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[file picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[Dateihandler]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
[Spezielle Ordner]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[special folders]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[Notizen-API]: integrate-with-onenote.md
[Notes API]: integrate-with-onenote.md
[Excel-API]: /graph/api/resources/excel?view=graph-rest-1.0
[Excel API]: /graph/api/resources/excel?view=graph-rest-1.0
[REST API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[Delta-API]: /graph/api/driveitem-delta?view=graph-rest-1.0
[delta API]: /graph/api/driveitem-delta?view=graph-rest-1.0
[Video]: /graph/api/resources/video?view=graph-rest-1.0
[video]: /graph/api/resources/video?view=graph-rest-1.0
[Foto]: /graph/api/resources/photo?view=graph-rest-1.0
[photo]: /graph/api/resources/photo?view=graph-rest-1.0
[Audio]: /graph/api/resources/audio?view=graph-rest-1.0
[audio]: /graph/api/resources/audio?view=graph-rest-1.0
[Formate]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[formats]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[Miniaturansichten]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[thumbnails]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[Vorschau]: /graph/api/driveitem-preview?view=graph-rest-beta
[preview]: /graph/api/driveitem-preview?view=graph-rest-beta
[Webhooks]: /graph/api/resources/webhooks?view=graph-rest-1.0
[webhooks]: /graph/api/resources/webhooks?view=graph-rest-1.0
[Drive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
