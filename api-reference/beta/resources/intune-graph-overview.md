---
title: Verwenden der Graph-API für Intune
description: " Hybridbereitstellungen Intune werden nicht unterstützt. "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062985"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="50e81-103">Arbeiten mit Intune in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50e81-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="50e81-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50e81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50e81-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50e81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50e81-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="50e81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="50e81-107">Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="50e81-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="50e81-108">In Szenarien für die Verwaltung mobiler Geräte (MDM, Mobile Device Management) unterstützt die Graph-API für Intune eigenständige Bereitstellungen. [Hybride Intune-Bereitstellungen](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50e81-108">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="50e81-109">Verwenden der Graph-API für Intune</span><span class="sxs-lookup"><span data-stu-id="50e81-109">Using the Intune Graph API</span></span>

<span data-ttu-id="50e81-110">Intune stellt Daten in der Microsoft Graph die gleiche Weise wie andere Cloud-Dienste, mit umfassenden Entität Informationen und Beziehung Navigation.</span><span class="sxs-lookup"><span data-stu-id="50e81-110">Intune provides data into the Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="50e81-111">Verwenden Sie Microsoft Graph zum Kombinieren von Informationen aus anderen Dienste und Intune für IT-Experten oder Endbenutzer rich Cross-dienstanwendungen erstellen.</span><span class="sxs-lookup"><span data-stu-id="50e81-111">  Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="50e81-112">Das Beispiel unten demonstriert, wie Sie herausfinden können, ob auf dem Gerät eines Benutzers eine bestimmte Anwendung installiert ist:</span><span class="sxs-lookup"><span data-stu-id="50e81-112">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="50e81-113">Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind:</span><span class="sxs-lookup"><span data-stu-id="50e81-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="50e81-114">Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="50e81-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="50e81-115">Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="50e81-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a><span data-ttu-id="50e81-116">Verwenden von berechtigungsbereiche Diagramm</span><span class="sxs-lookup"><span data-stu-id="50e81-116">Using Graph permission scopes</span></span>

<span data-ttu-id="50e81-117">Microsoft Graph steuert den Zugriff auf Ressourcen unter Verwendung von berechtigungsbereiche.</span><span class="sxs-lookup"><span data-stu-id="50e81-117">Microsof Graph controls access to resources using permission scopes.</span></span> <span data-ttu-id="50e81-118">Als Entwickler müssen Sie die Berechtigungsbereiche angeben, die Sie für den Zugriff auf Intune-Ressourcen benötigen.</span><span class="sxs-lookup"><span data-stu-id="50e81-118">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="50e81-119">In der Regel geben Sie die benötigten Berechtigungsbereiche im Azure Active Directory-Portal an.</span><span class="sxs-lookup"><span data-stu-id="50e81-119">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="50e81-120">Weitere Informationen finden Sie im Artikel zu den Themen [Microsoft Graph-Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) und [Intune-Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span><span class="sxs-lookup"><span data-stu-id="50e81-120">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a><span data-ttu-id="50e81-121">Mithilfe des Inhaltsverzeichnisses auf der Website Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50e81-121">To use the Table of Contents on the Microsoft Graph site</span></span>
  
<span data-ttu-id="50e81-122">Sie können das Inhaltsverzeichnis (im linken Bereich der Website) durchsuchen, um die Teile der Dokumentation Intune Diagramm-API und Ressource zu suchen, die Sie anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="50e81-122">You can browse the Table of Contents (in the left pane of the site) to find the parts of the Intune Graph API and resource documentation you want to see.</span></span>

1. <span data-ttu-id="50e81-123">Klicken Sie auf **/Beta Verweis** um Beta-Dokumente zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="50e81-123">Click **/Beta Reference** to open the beta docs.</span></span>
2. <span data-ttu-id="50e81-124">Führen Sie einen Bildlauf nach unten, und klicken Sie auf **Intune**.</span><span class="sxs-lookup"><span data-stu-id="50e81-124">Scroll down and click **Intune**.</span></span>
3. <span data-ttu-id="50e81-125">Unterabschnitten unter **Intune** für die Teile der API klicken Sie weiterhin auf Sie</span><span class="sxs-lookup"><span data-stu-id="50e81-125">Continue to click subsections below **Intune** for the parts of the API you</span></span> 
