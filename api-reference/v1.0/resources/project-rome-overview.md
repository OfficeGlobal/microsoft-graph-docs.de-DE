---
title: Verwenden Sie die Microsoft Graph-API Project ROM entwickelt
description: Project-ROM handelt es sich um eine Microsoft-Initiative zum Erstellen eines Cross-Geräts Plattform auftritt. Project-ROM ermöglicht einer app auf einem lokalen Client oder Dienst zur Interaktion mit apps und Dienste auf einem remote-Host, wenn der Benutzer mit der gleichen Microsoft-Konto signiert, mit denen sie auf dem Clientgerät anmelden. Dies ermöglicht es Ihnen zu Programm Cross-Gerät und plattformübergreifende Erfahrungen, die um Benutzeraufgaben statt Geräte zentriert werden.
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840964"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="0d80d-105">Verwenden Sie die Microsoft Graph-API Project ROM entwickelt</span><span class="sxs-lookup"><span data-stu-id="0d80d-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="0d80d-106">[Project-ROM](https://developer.microsoft.com/en-us/windows/project-rome) handelt es sich um eine Microsoft-Initiative zum Erstellen eines Cross-Geräts Plattform auftritt.</span><span class="sxs-lookup"><span data-stu-id="0d80d-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="0d80d-107">Project-ROM ermöglicht einer app auf einem lokalen Client oder Dienst zur Interaktion mit apps und Dienste auf einem remote-Host, wenn der Benutzer mit der gleichen Microsoft-Konto signiert, mit denen sie auf dem Clientgerät anmelden.</span><span class="sxs-lookup"><span data-stu-id="0d80d-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="0d80d-108">Dies ermöglicht es Ihnen zu Programm Cross-Gerät und plattformübergreifende Erfahrungen, die um Benutzeraufgaben statt Geräte zentriert werden.</span><span class="sxs-lookup"><span data-stu-id="0d80d-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="0d80d-109">Eine wichtige Komponente wird über Microsoft Graph so ermöglicht es den verfügbar gemacht: Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="0d80d-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="0d80d-110">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="0d80d-110">Activities</span></span>

<span data-ttu-id="0d80d-111">Aktivitäten in Microsoft Graph können Sie zu Laufwerk Benutzer mit Ihren apps für Geräte und Plattformen.</span><span class="sxs-lookup"><span data-stu-id="0d80d-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="0d80d-112">Eine Aktivität ist die Einheit eines Auftrags für Benutzer und besteht aus drei Komponenten:</span><span class="sxs-lookup"><span data-stu-id="0d80d-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="0d80d-113">Deep-link</span><span class="sxs-lookup"><span data-stu-id="0d80d-113">A deep link</span></span>
- <span data-ttu-id="0d80d-114">Eine visuelle Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d80d-114">A visual representation</span></span>
- <span data-ttu-id="0d80d-115">Metadaten, die die Aktivität beschreibt mithilfe der [https://schema.org/](https://schema.org/) shared Vokabular</span><span class="sxs-lookup"><span data-stu-id="0d80d-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="0d80d-116">Wenn eine Sitzung von einer Anwendung erstellt wird, wird die Aktivität des Berichtszeitraums Benutzer Engagements entsprechend ein Historienelement hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0d80d-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="0d80d-117">Jedes Mal wird ein Benutzer mit einer Aktivität reengages, ein neues Historienelement die Aktivität fällig Engagements Benutzer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0d80d-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="0d80d-118">Wenn eine Anwendung Aktivität Benutzerobjekte veröffentlicht, wird das Objekt in einigen der neuen Benutzeroberfläche Flächen in Windows angezeigt; Cortana Benachrichtigungen und Zeitachsen.</span><span class="sxs-lookup"><span data-stu-id="0d80d-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="0d80d-119">Sie können in Ihrer Aktivität-Objekten rich-Metadaten (zum Aktivitäten im richtigen Kontext dargestellt werden können) und rich visuelle Objekte (mit [Adaptive Karte](https://adaptivecards.io/) Markup) angeben.</span><span class="sxs-lookup"><span data-stu-id="0d80d-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="0d80d-120">Die folgenden Microsoft Graph-APIs können zum Erstellen und die Benutzeraktivitäten abrufen:</span><span class="sxs-lookup"><span data-stu-id="0d80d-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="0d80d-121">Erstellen oder Ersetzen Sie die Aktivität</span><span class="sxs-lookup"><span data-stu-id="0d80d-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="0d80d-122">Abrufen von Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="0d80d-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="0d80d-123">Aktuelle Aktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="0d80d-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="0d80d-124">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="0d80d-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="0d80d-125">Verlaufselement erstellen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="0d80d-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- <span data-ttu-id="0d80d-126">[Verlaufselement](../api/projectrome-delete-historyitem.md) löschen</span><span class="sxs-lookup"><span data-stu-id="0d80d-126">[Delete a history item](../api/projectrome-delete-historyitem.md)</span></span>

