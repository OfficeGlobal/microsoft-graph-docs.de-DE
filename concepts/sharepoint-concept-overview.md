---
title: Übersicht über SharePoint-Websites und die Inhalts-API
description: SharePoint ist Ihr mobiles, intelligentes Intranet. Mit SharePoint können Benutzer Inhalte. Wissen und Anwendungen freigeben und verwalten, um Gruppenarbeit zu stärken, Informationen zu finden und in der Organisation zusammenzuarbeiten. In Microsoft Graph können Sie die REST-API für SharePoint verwenden, um Ihre Lösungen in SharePoint-Websites und -Inhalte zu integrieren.
ms.openlocfilehash: e71ef735cadf13ddb05799431fcf74ae9b3fa463
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092300"
---
# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="7e668-105">Übersicht über SharePoint-Websites und die Inhalts-API</span><span class="sxs-lookup"><span data-stu-id="7e668-105">SharePoint sites and content API overview</span></span>

<span data-ttu-id="7e668-106">SharePoint ist Ihr mobiles, intelligentes Intranet.</span><span class="sxs-lookup"><span data-stu-id="7e668-106">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="7e668-107">Mit SharePoint können Benutzer Inhalte. Wissen und Anwendungen freigeben und verwalten, um Gruppenarbeit zu stärken, Informationen zu finden und in der Organisation zusammenzuarbeiten.</span><span class="sxs-lookup"><span data-stu-id="7e668-107">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="7e668-108">In Microsoft Graph können Sie die REST-API für SharePoint verwenden, um Ihre Lösungen in SharePoint-Websites und -Inhalte zu integrieren.</span><span class="sxs-lookup"><span data-stu-id="7e668-108">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="7e668-109">Warum die Integration in SharePoint-Websites und -Inhalte?</span><span class="sxs-lookup"><span data-stu-id="7e668-109">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="7e668-110">SharePoint-Websites unterstützen die Kommunikation und Zusammenarbeit im Team.</span><span class="sxs-lookup"><span data-stu-id="7e668-110">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="7e668-111">Office 365-Gruppen, Microsoft Teams und Portale basieren alle auf SharePoint, Sie können daher Microsoft Graph verwenden, um auf Daten zuzugreifen, unabhängig davon, wo diese gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="7e668-111">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="7e668-112">Verwenden Sie die SharePoint-API in Microsoft Graph für den Zugriff auf:</span><span class="sxs-lookup"><span data-stu-id="7e668-112">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="7e668-113">Teamwebsites, die die Inhalte speichern, an denen Benutzer mit ihren Kollegen zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="7e668-113">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="7e668-114">Kommunikationswebsites und Portale, in denen Benutzer vielfältige Inhaltsseiten veröffentlichen, die in der gesamten Organisation freigegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7e668-114">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="7e668-115">Nutzen von Daten mit SharePoint-Listen</span><span class="sxs-lookup"><span data-stu-id="7e668-115">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="7e668-116">[Lists][list] sind die Grundlage für die Datenspeicherung in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e668-116">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="7e668-117">[Create lists][create] zum Speichern einer Vielzahl von Unternehmensdaten, von einer einfachen Kundenkontaktliste hin zu einer benutzerdefinierten Unternehmensanwendung, bereitgestellt von PowerApps.</span><span class="sxs-lookup"><span data-stu-id="7e668-117">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="7e668-118">Bei Verwendung von [Spalten][] zum Definieren Ihres Schemas, kann SharePoint die Integrität Ihrer Daten schützen und auch Funktionen für eine umfassende Indizierung, Abfragen und Suche aktivieren.</span><span class="sxs-lookup"><span data-stu-id="7e668-118">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="7e668-119">Erweitern der Leistungsfähigkeit von Listen auf Dateien Ihres Teams</span><span class="sxs-lookup"><span data-stu-id="7e668-119">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="7e668-120">SharePoint speichert Dateien in einem speziellen [Listentyp][], der als Dokumentbibliothek bezeichnet wird.</span><span class="sxs-lookup"><span data-stu-id="7e668-120">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="7e668-121">Sie können die [OneDrive-API][] zum Arbeiten mit einer Bibliothek als [Laufwerk][] verwenden oder die SharePoint-API zum Arbeiten damit als [Liste][].</span><span class="sxs-lookup"><span data-stu-id="7e668-121">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="7e668-122">Genau wie eine normale Liste können Sie das Schema einer Dokumentbibliothek so erweitern, dass Ihre Unternehmensanforderungen mit benutzerdefinierten Spalten unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="7e668-122">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="7e668-123">Erweitern Sie Ihre App mit den SharePoint-Intranetdaten Ihrer Benutzer</span><span class="sxs-lookup"><span data-stu-id="7e668-123">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="7e668-124">Mit Microsoft Graph können Sie die wichtigsten Daten Ihrer Benutzer innerhalb Ihrer App anzeigen.</span><span class="sxs-lookup"><span data-stu-id="7e668-124">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="7e668-125">Aktualisieren Sie die Inhalte regelmäßig, indem Sie die Liste [abfragen][], in der die Daten Ihrer Benutzer gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="7e668-125">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="7e668-126">[Erstellen Sie][] eigene Listen für Ihre App und lassen Sie Benutzer auf Ihre daten in anderen SharePoint-Oberflächen zugreifen, oder blenden Sie Elemente aus.</span><span class="sxs-lookup"><span data-stu-id="7e668-126">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="7e668-127">Verwenden von Microsoft Graph zum Erweitern von SharePoint</span><span class="sxs-lookup"><span data-stu-id="7e668-127">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="7e668-128">SharePoint bietet als Plattform verschiedene Modelle für die Erweiterung und Integration:</span><span class="sxs-lookup"><span data-stu-id="7e668-128">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="7e668-129">Das [SharePoint Framework][] bietet eine Möglichkeit zum Erstellen von Webparts mithilfe von clientseitigen Technologien und Open Source-Tools, die auf SharePoint-Seiten gehostet werden können.</span><span class="sxs-lookup"><span data-stu-id="7e668-129">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="7e668-130">[SharePoint-Add-Ins][] sind eigenständige Erweiterungen, die einer SharePoint-Website hinzugefügt werden können, ohne dass benutzerdefinierter Code auf dem Server ausgeführt werden muss.</span><span class="sxs-lookup"><span data-stu-id="7e668-130">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="7e668-131">Wenn die App innerhalb einer SharePoint-Seite ausgeführt wird, können Sie problemlos Microsoft Graph verwenden, um auf die Daten über Office 365 hinweg zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="7e668-131">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="7e668-132">Weitere Details zu diesen Modellen finden Sie im [SharePoint Dev Center][] oder in den [SharePoint Developer-Dokumenten][].</span><span class="sxs-lookup"><span data-stu-id="7e668-132">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="api-reference"></a><span data-ttu-id="7e668-133">API-Referenz</span><span class="sxs-lookup"><span data-stu-id="7e668-133">API reference</span></span>
<span data-ttu-id="7e668-134">Suchen Sie die API-Referenz für diesen Dienst?</span><span class="sxs-lookup"><span data-stu-id="7e668-134">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="7e668-135">SharePoint-API in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="7e668-135">SharePoint API in Microsoft Graph v1.0</span></span>](/graph/api/resources/sharepoint?view=graph-rest-1.0)
- [<span data-ttu-id="7e668-136">SharePoint-API in Microsoft Graph, Betaversion</span><span class="sxs-lookup"><span data-stu-id="7e668-136">SharePoint API in Microsoft Graph beta</span></span>](/graph/api/resources/sharepoint?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="7e668-137">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7e668-137">Next steps</span></span>

<span data-ttu-id="7e668-138">Erste Schritte mit SharePoint in Microsoft Graph, indem Sie mehr über das [Arbeiten mit Websites][SharePoint] erfahren.</span><span class="sxs-lookup"><span data-stu-id="7e668-138">Get started with SharePoint in Microsoft Graph by learning more about [working with sites][SharePoint].</span></span>

[list]: /graph/api/resources/list?view=graph-rest-1.0
[columns]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[list type]: /graph/api/resources/listinfo?view=graph-rest-1.0
[create]: /graph/api/list-create?view=graph-rest-1.0
[querying]: /graph/api/listitem-get?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[OneDrive-API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[OneDrive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint-Add-Ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[SharePoint Developer-Dokumente]: https://aka.ms/spdev-docs
[SharePoint Developer Docs]: https://aka.ms/spdev-docs
[SharePoint]: /graph/api/resources/sharepoint?view=graph-rest-1.0
