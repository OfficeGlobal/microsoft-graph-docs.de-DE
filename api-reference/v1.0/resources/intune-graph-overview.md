---
title: Verwenden der Graph-API für Intune
description: " Hybridbereitstellungen Intune werden nicht unterstützt. "
ms.openlocfilehash: 23f6550fca708b64357b7b5132a2a42060cfa4bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27015981"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="a5ef8-103">Arbeiten mit Intune in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a5ef8-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="a5ef8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a5ef8-105">Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="a5ef8-106">In Szenarien für die Verwaltung mobiler Geräte (MDM, Mobile Device Management) unterstützt die Graph-API für Intune eigenständige Bereitstellungen. [Hybride Intune-Bereitstellungen](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-106">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="a5ef8-107">Verwenden der Graph-API für Intune</span><span class="sxs-lookup"><span data-stu-id="a5ef8-107">Using the Intune Graph API</span></span>

<span data-ttu-id="a5ef8-108">Intune stellt Daten auf die gleiche Weise für die Microsoft Graph-API bereit, wie es auch andere Clouddienste tun, mit detaillierten Informationen zu Entitäten und Möglichkeiten zur Beziehungsnavigation.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="a5ef8-109">Mithilfe der Microsoft Graph-API können Sie Informationen aus anderen Diensten und aus Intune miteinander kombinieren und so funktionsreiche, dienstübergreifende Anwendungen für IT-Experten oder Endbenutzer erstellen.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-109">  Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="a5ef8-110">Das Beispiel unten demonstriert, wie Sie herausfinden können, ob auf dem Gerät eines Benutzers eine bestimmte Anwendung installiert ist:</span><span class="sxs-lookup"><span data-stu-id="a5ef8-110">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="a5ef8-111">Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind:</span><span class="sxs-lookup"><span data-stu-id="a5ef8-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="a5ef8-112">Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="a5ef8-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="a5ef8-113">Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="a5ef8-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a><span data-ttu-id="a5ef8-114">Verwenden von Berechtigungsbereichen</span><span class="sxs-lookup"><span data-stu-id="a5ef8-114">Using permission scopes</span></span>

<span data-ttu-id="a5ef8-115">Die Microsoft Graph-API steuert den Zugriff auf Ressourcen mithilfe von Berechtigungsbereichen.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-115">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="a5ef8-116">Als Entwickler müssen Sie die Berechtigungsbereiche angeben, die Sie für den Zugriff auf Intune-Ressourcen benötigen.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-116">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="a5ef8-117">In der Regel geben Sie die benötigten Berechtigungsbereiche im Azure Active Directory-Portal an.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-117">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="a5ef8-118">Weitere Informationen finden Sie im Artikel zu den Themen [Microsoft Graph-Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) und [Intune-Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span><span class="sxs-lookup"><span data-stu-id="a5ef8-118">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a5ef8-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="a5ef8-119">Next Steps</span></span>

- <span data-ttu-id="a5ef8-120">Erfahren Sie, [wie Sie mit Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) , um die Microsoft Graph-API für Intune zugreifen.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="a5ef8-121">Machen Sie sich die [PowerShell Intune Beispiele](https://github.com/microsoftgraph/powershell-intune-samples), die zeigen, wie Diagramm-API für Intune im Kontext des Beispiele verwenden.</span><span class="sxs-lookup"><span data-stu-id="a5ef8-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use Graph API for Intune in context of working examples.</span></span>