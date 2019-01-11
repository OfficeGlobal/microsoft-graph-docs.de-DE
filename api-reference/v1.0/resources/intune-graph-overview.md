---
title: Verwenden der Graph-API für Intune
description: " Hybridbereitstellungen Intune werden nicht unterstützt. "
author: tfitzmac
localization_priority: Priority
ms.openlocfilehash: 1222f064b075c8884f5c66c101ae0e15256221c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830681"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="a0895-103">Arbeiten mit Intune in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a0895-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="a0895-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="a0895-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a0895-105">Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="a0895-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="a0895-106">Für mobiles Gerät Verwaltungsszenarien (MDM) unterstützt der Microsoft Graph-API für Intune Standalone-Bereitstellungen. Intune [hybridbereitstellungen](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0895-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="a0895-107">Verwenden das Microsoft Graph-API für Intune</span><span class="sxs-lookup"><span data-stu-id="a0895-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="a0895-108">Intune stellt Daten auf die gleiche Weise für die Microsoft Graph-API bereit, wie es auch andere Clouddienste tun, mit detaillierten Informationen zu Entitäten und Möglichkeiten zur Beziehungsnavigation.</span><span class="sxs-lookup"><span data-stu-id="a0895-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="a0895-109">Verwenden Sie die Microsoft Graph-API zum Kombinieren von Informationen aus anderen Dienste und Intune für IT-Experten oder Endbenutzer rich Cross-dienstanwendungen erstellen.</span><span class="sxs-lookup"><span data-stu-id="a0895-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="a0895-110">Das folgende Beispiel zeigt, wie Sie ermitteln können, ob eine Anwendung auf das Gerät des Benutzers installiert ist:</span><span class="sxs-lookup"><span data-stu-id="a0895-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="a0895-111">Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind:</span><span class="sxs-lookup"><span data-stu-id="a0895-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="a0895-112">Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="a0895-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="a0895-113">Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="a0895-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a><span data-ttu-id="a0895-114">Verwenden von Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0895-114">Using permissions</span></span>

<span data-ttu-id="a0895-115">Die Microsoft Graph-API steuert den Zugriff auf Ressourcen über Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="a0895-115">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="a0895-116">Als Entwickler müssen Sie die Berechtigungen angeben, die Sie Intune-Ressourcen zugreifen müssen.</span><span class="sxs-lookup"><span data-stu-id="a0895-116">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="a0895-117">Geben Sie in der Regel die Berechtigungen im Azure Active Directory-Portal.</span><span class="sxs-lookup"><span data-stu-id="a0895-117">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="a0895-118">Weitere Informationen finden Sie unter [Microsoft Graph Berechtigungen Verweis](https://docs.microsoft.com/en-us/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0895-118">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a0895-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="a0895-119">Next Steps</span></span>

- <span data-ttu-id="a0895-120">Erfahren Sie, [wie Sie mit Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) , um die Microsoft Graph-API für Intune zugreifen.</span><span class="sxs-lookup"><span data-stu-id="a0895-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="a0895-121">Machen Sie sich die [PowerShell Intune Beispiele](https://github.com/microsoftgraph/powershell-intune-samples), die zeigen, wie die Microsoft Graph-API für Intune im Kontext des Beispiele verwenden.</span><span class="sxs-lookup"><span data-stu-id="a0895-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
