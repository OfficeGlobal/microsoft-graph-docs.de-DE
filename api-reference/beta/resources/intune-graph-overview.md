---
title: Verwenden der Intune Graph API – Microsoft Graph-API
description: Listet die Endpunkte der Microsoft Graph-API für Intune (REST) auf, mit denen Sie Ihre Mandantenorganisation, deren Geräte, Apps, Zugriff und Ressourcen verwalten können.
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: fc254772a5b4db131a5cda45fc83b336bf12f993
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167445"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="f7b98-103">Arbeiten mit Intune in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f7b98-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="f7b98-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7b98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7b98-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7b98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7b98-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/de-DE/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="f7b98-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/de-DE/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="f7b98-107">Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="f7b98-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="f7b98-108">In Szenarien für die Verwaltung mobiler Geräte (MDM, Mobile Device Management) unterstützt die Microsoft Graph-API für Intune eigenständige Bereitstellungen. [Hybride Intune-Bereitstellungen](https://docs.microsoft.com/de-DE/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7b98-108">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/de-DE/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="f7b98-109">Verwenden der Microsoft Graph-API für Intune</span><span class="sxs-lookup"><span data-stu-id="f7b98-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="f7b98-110">Intune stellt Daten auf die gleiche Weise für Microsoft Graph bereit, wie es auch andere Clouddienste tun, mit detaillierten Informationen zu Entitäten und Möglichkeiten zur Beziehungsnavigation.</span><span class="sxs-lookup"><span data-stu-id="f7b98-110">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="f7b98-111">Mithilfe von Microsoft Graph können Sie Informationen aus anderen Diensten und aus Intune miteinander kombinieren und so funktionsreiche, dienstübergreifende Anwendungen für IT-Experten oder Endbenutzer erstellen.</span><span class="sxs-lookup"><span data-stu-id="f7b98-111">Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="f7b98-112">Das folgende Beispiel demonstriert, wie Sie herausfinden können, ob auf dem Gerät eines Benutzers eine bestimmte Anwendung installiert ist:</span><span class="sxs-lookup"><span data-stu-id="f7b98-112">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="f7b98-113">Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind:</span><span class="sxs-lookup"><span data-stu-id="f7b98-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="f7b98-114">Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="f7b98-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="f7b98-115">Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="f7b98-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="f7b98-116">Verwenden von Microsoft Graph-Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7b98-116">Microsoft Graph permissions</span></span>

<span data-ttu-id="f7b98-117">Microsoft Graph steuert den Zugriff auf Ressourcen über Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="f7b98-117">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="f7b98-118">Als Entwickler müssen Sie die Berechtigungen angeben, die Sie für den Zugriff auf Intune-Ressourcen benötigen.</span><span class="sxs-lookup"><span data-stu-id="f7b98-118">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="f7b98-119">In der Regel geben Sie die Berechtigungen im Azure Active Directory-Portal an.</span><span class="sxs-lookup"><span data-stu-id="f7b98-119">Typically, you specify permissions in the Azure Active Directory (Azure AD) portal.</span></span> <span data-ttu-id="f7b98-120">Weitere Informationen finden Sie in der [Referenz zu den Microsoft Graph-Berechtigungen](https://docs.microsoft.com/de-DE/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7b98-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/de-DE/graph/permissions-reference) and Reports permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f7b98-121">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f7b98-121">Next Steps</span></span>

- <span data-ttu-id="f7b98-122">Erfahren Sie [wie Sie Azure AD verwenden](https://docs.microsoft.com/de-DE/intune/intune-graph-apis), um auf die Microsoft Graph-API für Intune zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="f7b98-122">Learn [how to use Azure AD](https://docs.microsoft.com/de-DE/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="f7b98-123">Erkunden Sie die [PowerShell Intune-Beispiele](https://github.com/microsoftgraph/powershell-intune-samples), die zeigen, wie Sie die Microsoft Graph-API für Intune im Kontext von Arbeitsbeispielen verwenden können.</span><span class="sxs-lookup"><span data-stu-id="f7b98-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

