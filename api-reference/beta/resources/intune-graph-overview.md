---
title: Verwenden der Graph-API für Intune
description: " Hybridbereitstellungen Intune werden nicht unterstützt. "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 1db77aceaab82e869fc540d2b29cce17ddba100f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911952"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="57a87-103">Arbeiten mit Intune in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="57a87-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="57a87-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="57a87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57a87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57a87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57a87-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="57a87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="57a87-107">Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="57a87-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="57a87-108">Für mobiles Gerät Verwaltungsszenarien (MDM) unterstützt der Microsoft Graph-API für Intune Standalone-Bereitstellungen. Intune [hybridbereitstellungen](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57a87-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="57a87-109">Verwenden das Microsoft Graph-API für Intune</span><span class="sxs-lookup"><span data-stu-id="57a87-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="57a87-110">Intune stellt Daten in Microsoft Graph die gleiche Weise wie andere Cloud-Dienste, mit umfassenden Entität Informationen und Beziehung Navigation.</span><span class="sxs-lookup"><span data-stu-id="57a87-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="57a87-111">Verwenden Sie Microsoft Graph zum Kombinieren von Informationen aus anderen Dienste und Intune für IT-Experten oder Endbenutzer rich Cross-dienstanwendungen erstellen.</span><span class="sxs-lookup"><span data-stu-id="57a87-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="57a87-112">Das folgende Beispiel zeigt, wie Sie ermitteln können, ob eine Anwendung auf das Gerät des Benutzers installiert ist:</span><span class="sxs-lookup"><span data-stu-id="57a87-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="57a87-113">Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind:</span><span class="sxs-lookup"><span data-stu-id="57a87-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="57a87-114">Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="57a87-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="57a87-115">Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="57a87-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="57a87-116">Verwenden von Microsoft Graph-Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="57a87-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="57a87-117">Microsoft Graph steuert den Zugriff auf Ressourcen über Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="57a87-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="57a87-118">Als Entwickler müssen Sie die Berechtigungen angeben, die Sie Intune-Ressourcen zugreifen müssen.</span><span class="sxs-lookup"><span data-stu-id="57a87-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="57a87-119">Geben Sie in der Regel die Berechtigungen im Azure Active Directory-Portal.</span><span class="sxs-lookup"><span data-stu-id="57a87-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="57a87-120">Weitere Informationen finden Sie unter [Microsoft Graph Berechtigungen Verweis](https://docs.microsoft.com/en-us/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a87-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="57a87-121">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="57a87-121">Next Steps</span></span>

- <span data-ttu-id="57a87-122">Erfahren Sie, [wie Sie mit Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) , um die Microsoft Graph-API für Intune zugreifen.</span><span class="sxs-lookup"><span data-stu-id="57a87-122">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="57a87-123">Machen Sie sich die [PowerShell Intune Beispiele](https://github.com/microsoftgraph/powershell-intune-samples), die zeigen, wie die Microsoft Graph-API für Intune im Kontext des Beispiele verwenden.</span><span class="sxs-lookup"><span data-stu-id="57a87-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

