---
title: Überblick über Intune-Geräte und die Apps-API
description: 'Mit Microsoft Intune können Unternehmen Geräte und Apps verwalten. Sie können mit der Intune-API in Microsoft Graph Geräte und Apps verwalten sowie Intune mit en von Ihnen bevorzugten Tools konfigurieren. '
ms.openlocfilehash: fced71d317aa5f2aebfd2c44237ea9087a6be4f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092284"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="c84a8-104">Überblick über Intune-Geräte und die Apps-API</span><span class="sxs-lookup"><span data-stu-id="c84a8-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="c84a8-105">Mit Microsoft Intune können Unternehmen Geräte und Apps verwalten.</span><span class="sxs-lookup"><span data-stu-id="c84a8-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="c84a8-106">Sie können mit der Intune-API in Microsoft Graph Geräte und Apps verwalten sowie Intune mit en von Ihnen bevorzugten Tools konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="c84a8-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="c84a8-107">Wenn Sie ein ISV sind, können Sie mit der Intune-API auch Kundenmandanten verwalten.</span><span class="sxs-lookup"><span data-stu-id="c84a8-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

## <a name="why-integrate-with-intune"></a><span data-ttu-id="c84a8-108">Gründe für die Integration mit Intune</span><span class="sxs-lookup"><span data-stu-id="c84a8-108">Why integrate with Intune?</span></span>

<span data-ttu-id="c84a8-109">Sie können die Intune-API in Microsoft Graph verwenden, um auf Intune Geräte- und -Anwendungsinformationen zuzugreifen, Geräte und Apps zu verwalten und Intune zu automatisieren.</span><span class="sxs-lookup"><span data-stu-id="c84a8-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="c84a8-110">Verwalten von Geräten</span><span class="sxs-lookup"><span data-stu-id="c84a8-110">Manage devices</span></span>

<span data-ttu-id="c84a8-111">Die Intune-API bietet Ihnen die folgenden Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="c84a8-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="c84a8-112">Definieren und Durchsetzen von [Geräte-Compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)-Richtlinien, wie z. B. Komplexität und Lebensdauer von Kennwörtern, Verschlüsselung, Bedrohungsschutzstufen usw.</span><span class="sxs-lookup"><span data-stu-id="c84a8-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="c84a8-113">(Welche Richtlinien unterstützt werden, hängt vom Betriebssystem und der Version ab.)</span><span class="sxs-lookup"><span data-stu-id="c84a8-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="c84a8-114">[Schützen von Unternehmensdaten](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), und zwar unabhängig davon, ob die Geräteplattform Windows, Android, Mac oder iOS ist.</span><span class="sxs-lookup"><span data-stu-id="c84a8-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="c84a8-115">Erstellen und Bereitstellen von [Gerätekonfigurationsrichtlinien](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), einschließlich Betriebssystemplattform/-versionierung, Domänenmitgliedschaft und Verwaltung von Konfigurationseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="c84a8-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="c84a8-116">Erstellen und Bereitstellen der [Zugriffssteuerungsrichtlinien](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) für Geräte, einschließlich eingeschränktem Download, Zugriff auf Netzwerkgeräte und Dateiübertragung.</span><span class="sxs-lookup"><span data-stu-id="c84a8-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="c84a8-117">Durchführen von [Remote-Aktionen](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), wie z. B. das Lokalisieren von Geräten, Ändern von Kennwörtern und Löschen von Gerätedaten.</span><span class="sxs-lookup"><span data-stu-id="c84a8-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="c84a8-118">Verwalten von Apps</span><span class="sxs-lookup"><span data-stu-id="c84a8-118">Manage apps</span></span> 

<span data-ttu-id="c84a8-119">Mit der Intune-API können Sie die folgenden Aufgaben für die App-Verwaltung ausführen:</span><span class="sxs-lookup"><span data-stu-id="c84a8-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="c84a8-120">Bereitstellen von [Apps auf Geräten](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) oder das Bereitstellen von Apps verhindern.</span><span class="sxs-lookup"><span data-stu-id="c84a8-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="c84a8-121">Verwalten des Zugriffs auf [e-Books](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) und zugehörige Dienste.</span><span class="sxs-lookup"><span data-stu-id="c84a8-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="c84a8-122">Definieren und Bereitstellen von App-Konfigurationseinstellungen, Einstellungen für den App-Schutz und Verwendungsrichtlinien für Apps.</span><span class="sxs-lookup"><span data-stu-id="c84a8-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="c84a8-123">Automatisieren von Intune</span><span class="sxs-lookup"><span data-stu-id="c84a8-123">Automate Intune</span></span>

<span data-ttu-id="c84a8-124">Die Intune-API bietet die folgenden Automatisierungsfunktionen:</span><span class="sxs-lookup"><span data-stu-id="c84a8-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="c84a8-125">Definieren und Zuweisen von [rollenbasierten](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) Zugriffssteuerungen.</span><span class="sxs-lookup"><span data-stu-id="c84a8-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="c84a8-126">Prüfen der Compliance, Verwendung und des Zugriffs sowie entsprechende Berichterstattung.</span><span class="sxs-lookup"><span data-stu-id="c84a8-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="c84a8-127">Verwalten von [Telekommunikationsausgaben](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="c84a8-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="c84a8-128">API-Referenz</span><span class="sxs-lookup"><span data-stu-id="c84a8-128">API reference</span></span>
<span data-ttu-id="c84a8-129">Suchen Sie die API-Referenz für diesen Dienst?</span><span class="sxs-lookup"><span data-stu-id="c84a8-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="c84a8-130">Intune-API in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="c84a8-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="c84a8-131">Intune-API in Microsoft Graph, Betaversion</span><span class="sxs-lookup"><span data-stu-id="c84a8-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="c84a8-132">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="c84a8-132">Next steps</span></span>

- <span data-ttu-id="c84a8-133">[Verwenden von Azure AD für den Zugriff auf die Intune-API](https://docs.microsoft.com/intune/intune-graph-apis).</span><span class="sxs-lookup"><span data-stu-id="c84a8-133">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="c84a8-134">Informationen zum Ausführen allgemeiner Aufgaben mithilfe der [PowerShell-Intune-Beispiele](https://github.com/microsoftgraph/powershell-intune-samples).</span><span class="sxs-lookup"><span data-stu-id="c84a8-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="c84a8-135">Informationen zum [Verwenden der Intune-REST-API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="c84a8-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="c84a8-136">Informationen zu Neuerungen in der Intune-API finden Sie im [Changelog](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="c84a8-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="c84a8-137">In den [Beispielen](https://developer.microsoft.com/graph/graph/examples) finden Sie weitere Ideen für die Verwendung von Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c84a8-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
