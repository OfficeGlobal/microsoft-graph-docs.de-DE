---
title: Verwenden der Benachrichtigungs-REST-API in Microsoft Graph
description: Sie können die Benachrichtigungs-API in Microsoft Graph verwenden, um Pushbenachrichtigungen an einen Benutzer zu senden. Wählen Sie einfach ein Benutzerkonto aus, an das eine Benachrichtigung gesendet werden soll; die Plattform übermittelt die Benachrichtigung dann an alle Geräteendpunkte. Benachrichtigungs-API-Anfragen werden im Auftrag eines Benutzers über delegierte Berechtigungen und die [Benachrichtigungsberechtigung]( /graph/permissions_reference) ausgeführt, die mit Microsoft-Konten oder mit Geschäfts-oder Schulkonten verwendet werden können.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 2a4c23955e348159d2e17514d6041260f13cffba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513984"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="2313a-105">Verwenden der Benachrichtigungs-REST-API in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2313a-105">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2313a-106">Sie können die Benachrichtigungs-API in Microsoft Graph verwenden, um Pushbenachrichtigungen an einen Benutzer zu senden.</span><span class="sxs-lookup"><span data-stu-id="2313a-106">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="2313a-107">Wählen Sie einfach ein Benutzerkonto aus, an das eine Benachrichtigung gesendet werden soll; die Plattform übermittelt die Benachrichtigung dann an alle Geräteendpunkte.</span><span class="sxs-lookup"><span data-stu-id="2313a-107">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="2313a-108">Benachrichtigungs-API-Anfragen werden im Auftrag eines Benutzers über [delegierte Berechtigungen](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) und die [Benachrichtigungsberechtigung]( /graph/permissions_reference) ausgeführt, die mit Microsoft-Konten oder mit Geschäfts-oder Schulkonten verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2313a-108">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="2313a-109">Diese Art von benutzerzentrierter Benachrichtigung wird von der [notification](../resources/projectrome-notification.md)-Ressource dargestellt und wird in Microsoft Graph gespeichert.</span><span class="sxs-lookup"><span data-stu-id="2313a-109">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="2313a-110">Diese kann dann von der Veröffentlichungs-App über die [Project Rome-SDK-APIs](https://github.com/Microsoft/project-rome) geöffnet und verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="2313a-110">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="2313a-111">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2313a-111">Next steps</span></span>
- <span data-ttu-id="2313a-112">Sehen Sie sich die [notification-Ressource](../resources/projectrome-notification.md) an, und erstellen Sie Benachrichtigungen, um mit Ihren Benutzern zu interagieren.</span><span class="sxs-lookup"><span data-stu-id="2313a-112">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="2313a-113">Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.</span><span class="sxs-lookup"><span data-stu-id="2313a-113">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/notifications-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
