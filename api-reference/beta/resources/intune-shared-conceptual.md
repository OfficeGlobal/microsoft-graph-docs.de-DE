---
title: Gemeinsam genutzten Ressourcen in Microsoft Intune
description: Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.  Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.  Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.
ms.openlocfilehash: a0e896b2aed219679ec45804dc94b22b7cb9d727
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065565"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="67699-105">Gemeinsam genutzten Ressourcen in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="67699-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="67699-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67699-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67699-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67699-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67699-108">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="67699-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="67699-109">Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.</span><span class="sxs-lookup"><span data-stu-id="67699-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="67699-110">Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.</span><span class="sxs-lookup"><span data-stu-id="67699-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="67699-111">Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67699-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="67699-112">Die folgenden Ressourcen: Grafik werden sowohl Intune Workflows verwendet:</span><span class="sxs-lookup"><span data-stu-id="67699-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="67699-113">Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="67699-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="67699-114">allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67699-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="67699-115">allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67699-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="67699-116">Compliance-status</span><span class="sxs-lookup"><span data-stu-id="67699-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="67699-117">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67699-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="67699-118">Geräte-App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="67699-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="67699-119">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="67699-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="67699-120">Registrierung Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="67699-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="67699-121">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="67699-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="67699-122">Gerätetyp-Plattform</span><span class="sxs-lookup"><span data-stu-id="67699-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="67699-123">Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="67699-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="67699-124">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="67699-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="67699-125">exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67699-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="67699-126">groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67699-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="67699-127">Installieren Sie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="67699-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="67699-128">ipRange</span><span class="sxs-lookup"><span data-stu-id="67699-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="67699-129">iPv4Range</span><span class="sxs-lookup"><span data-stu-id="67699-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="67699-130">iPv6Range</span><span class="sxs-lookup"><span data-stu-id="67699-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="67699-131">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="67699-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="67699-132">MIME-Inhalt</span><span class="sxs-lookup"><span data-stu-id="67699-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="67699-133">proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="67699-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="67699-134">Report</span><span class="sxs-lookup"><span data-stu-id="67699-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="67699-135">reportRoot</span><span class="sxs-lookup"><span data-stu-id="67699-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="67699-136">Resultierende app-Status</span><span class="sxs-lookup"><span data-stu-id="67699-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="67699-137">RGB-Farbe</span><span class="sxs-lookup"><span data-stu-id="67699-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="67699-138">Führen Sie als Kontotyp</span><span class="sxs-lookup"><span data-stu-id="67699-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="67699-139">Führen Sie Zustand</span><span class="sxs-lookup"><span data-stu-id="67699-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="67699-140">Gespeichert von Benutzeroberflächenoptionen Zustand-Generierung</span><span class="sxs-lookup"><span data-stu-id="67699-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="67699-141">URI</span><span class="sxs-lookup"><span data-stu-id="67699-141">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="67699-142">User</span><span class="sxs-lookup"><span data-stu-id="67699-142">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="67699-143">VPP token Kontotyp</span><span class="sxs-lookup"><span data-stu-id="67699-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="67699-144">VPP token Aktion Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="67699-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="67699-145">Windows-Domäne Join-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="67699-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
