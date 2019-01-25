---
title: 'Verwenden Sie die Microsoft Graph-API Project ROM entwickelt '
description: 'Project-ROM ist eine Microsoft-Initiative eine Plattform zu erstellen, mit die app-Entwickler umfangreiche Cross-Gerät Erfahrungen erstellen können. Project-ROM kann verschiedene Funktionen, die verschiedene Dienste und Clientendpunkte verbinden, wenn der Benutzer bei sich mit den gleichen Microsoft-Konto oder arbeiten oder Schule Konto. Dadurch können Sie Cross-Gerät und plattformübergreifende Erfahrungen implementieren, die um Benutzeraufgaben statt Geräte zentriert wird. '
localization_priority: Normal
ms.openlocfilehash: 57c5189f3caf64ec048d000d5e9108811bd88145
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509693"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="5cf4a-105">Verwenden Sie die Microsoft Graph-API Project ROM entwickelt</span><span class="sxs-lookup"><span data-stu-id="5cf4a-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf4a-106">[Project-ROM](https://developer.microsoft.com/en-us/windows/project-rome) ist eine Microsoft-Initiative eine Plattform zu erstellen, mit die app-Entwickler umfangreiche Cross-Gerät Erfahrungen erstellen können.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="5cf4a-107">Project-ROM kann verschiedene Funktionen, die verschiedene Dienste und Clientendpunkte verbinden, wenn der Benutzer bei sich mit den gleichen Microsoft-Konto oder arbeiten oder Schule Konto.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="5cf4a-108">Dadurch können Sie Cross-Gerät und plattformübergreifende Erfahrungen implementieren, die um Benutzeraufgaben statt Geräte zentriert wird.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="5cf4a-109">Drei Schlüsselfunktionen Project ROM über Microsoft Graph zur einfacheren hervorragende Cross-Gerät Erfahrungen aktivieren verfügbar gemacht werden: Aktivitäten, Geräte und Benachrichtigungen.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="5cf4a-110">activities</span><span class="sxs-lookup"><span data-stu-id="5cf4a-110">Activities</span></span>

<span data-ttu-id="5cf4a-111">Aktivitäten in Microsoft Graph können Sie zu Laufwerk Benutzer mit Ihren apps für Geräte und Plattformen.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="5cf4a-112">Eine Aktivität ist die Einheit eines Auftrags für Benutzer und besteht aus drei Komponenten:</span><span class="sxs-lookup"><span data-stu-id="5cf4a-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="5cf4a-113">Deep-link</span><span class="sxs-lookup"><span data-stu-id="5cf4a-113">A deep link</span></span>
- <span data-ttu-id="5cf4a-114">Eine visuelle Darstellung</span><span class="sxs-lookup"><span data-stu-id="5cf4a-114">A visual representation</span></span>
- <span data-ttu-id="5cf4a-115">Metadaten, die die Aktivität beschreibt mithilfe der [https://schema.org/](https://schema.org/) shared Vokabular</span><span class="sxs-lookup"><span data-stu-id="5cf4a-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="5cf4a-116">Wenn eine Sitzung von einer Anwendung erstellt wird, wird die Aktivität des Berichtszeitraums Benutzer Engagements entsprechend ein Historienelement hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="5cf4a-117">Jedes Mal wird ein Benutzer mit einer Aktivität reengages, ein neues Historienelement die Aktivität fällig Engagements Benutzer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="5cf4a-118">Wenn eine Anwendung Aktivität Benutzerobjekte veröffentlicht, wird das Objekt in einigen der neuen Benutzeroberfläche Flächen in Windows angezeigt; Cortana Benachrichtigungen und Zeitachsen.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="5cf4a-119">Sie können in Ihrer Aktivität-Objekten rich-Metadaten (zum Aktivitäten im richtigen Kontext dargestellt werden können) und rich visuelle Objekte (mit [Adaptive Karte](https://adaptivecards.io/) Markup) angeben.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="5cf4a-120">Die folgenden Microsoft Graph-APIs können zum Erstellen und die Benutzeraktivitäten abrufen:</span><span class="sxs-lookup"><span data-stu-id="5cf4a-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="5cf4a-121">Erstellen oder Ersetzen Sie die Aktivität</span><span class="sxs-lookup"><span data-stu-id="5cf4a-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="5cf4a-122">Abrufen von Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="5cf4a-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="5cf4a-123">Aktuelle Aktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="5cf4a-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="5cf4a-124">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="5cf4a-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="5cf4a-125">Verlaufselement erstellen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="5cf4a-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- <span data-ttu-id="5cf4a-126">[Verlaufselement](../api/projectrome-delete-historyitem.md) löschen</span><span class="sxs-lookup"><span data-stu-id="5cf4a-126">[Delete a history item](../api/projectrome-delete-historyitem.md)</span></span>

## <a name="devices"></a><span data-ttu-id="5cf4a-127">Geräte</span><span class="sxs-lookup"><span data-stu-id="5cf4a-127">Devices</span></span>

<span data-ttu-id="5cf4a-128">Sie können Project-ROM-APIs in Microsoft Graph verwenden:</span><span class="sxs-lookup"><span data-stu-id="5cf4a-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="5cf4a-129">Entdecken Sie und Herstellen einer Verbindung des Benutzers Geräte mit</span><span class="sxs-lookup"><span data-stu-id="5cf4a-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="5cf4a-130">Starten Sie Remote apps auf diesen Geräten</span><span class="sxs-lookup"><span data-stu-id="5cf4a-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="5cf4a-131">Senden von Nachrichten an Ihre apps auf diesen Geräten</span><span class="sxs-lookup"><span data-stu-id="5cf4a-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="5cf4a-132">Mit diesen APIs können Sie apps erstellen, die umfangreiche Erfahrungen erstellen, die ein einzelnes Gerät transcend.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="5cf4a-133">Beispielsweise können Sie Ihre app So starten Sie auf einem größeren Bildschirm erweitern.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="5cf4a-134">Oder Sie können eine Mobile Begleit-Erfahrung für eine app auf einem anderen Geräte des Benutzers erstellen.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="5cf4a-135">Die folgenden Microsoft Graph-APIs können Sie die Kommunikation mit anderen Windows-Geräten:</span><span class="sxs-lookup"><span data-stu-id="5cf4a-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="5cf4a-136">Auflisten des Benutzers Geräte</span><span class="sxs-lookup"><span data-stu-id="5cf4a-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="5cf4a-137">Senden Sie einen Befehl zu einem Gerät</span><span class="sxs-lookup"><span data-stu-id="5cf4a-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="5cf4a-138">Abrufen des Befehlsstatus</span><span class="sxs-lookup"><span data-stu-id="5cf4a-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="5cf4a-139">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="5cf4a-139">Notifications</span></span>

<span data-ttu-id="5cf4a-140">Sie können die Benachrichtigungen APIs in Microsoft Graph Benachrichtigungen über mehrere Endpunkte übermittelt werden, die denselben Benutzer, in angemeldet ist verwenden.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-140">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="5cf4a-141">Sie können einen Benutzer direkt abzielen, beim Bereitstellen von Benachrichtigungen anstelle von Adressen/Gerätekanäle kümmern.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-141">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="5cf4a-142">Auf diese Weise können Sie auf die rechten Benachrichtigungsszenarien in einer Human-centric, statt eine Gerät-centric Möglichkeit entwerfen konzentrieren.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-142">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="5cf4a-143">Sie können eine Benachrichtigung Rohdaten oder eine direkte visuelle Benachrichtigung veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-143">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="5cf4a-144">Wenn eine Benachrichtigung über eine unformatierte Daten an einen Endpunkt Gerät übermittelt werden, können Sie die [Client-SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph-Benachrichtigungen SDK für Windows Project ROM SDK für iOS und Android) klicken Sie dann verwenden, empfangen und Benachrichtigungen verwalten.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-144">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="5cf4a-145">Wenn eine direkte visuelle Benachrichtigung an einen Endpunkt Gerät gesendet wird, wird die systemeigene plattformspezifische-Benachrichtigung an dem Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5cf4a-145">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="5cf4a-146">Weitere Informationen hierzu finden Sie unter [Erstellen und senden Sie eine Benachrichtigung](../api/projectrome-notification-post.md).</span><span class="sxs-lookup"><span data-stu-id="5cf4a-146">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/project-rome-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
