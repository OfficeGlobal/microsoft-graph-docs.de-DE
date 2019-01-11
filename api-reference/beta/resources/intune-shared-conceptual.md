---
title: Gemeinsam genutzten Ressourcen in Microsoft Intune
description: Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.  Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.  Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.
localization_priority: Normal
ms.openlocfilehash: c381ba84c9240a2b8e7428a3c055b8baf35fb243
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852626"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="d0c0d-105">Gemeinsam genutzten Ressourcen in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d0c0d-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="d0c0d-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d0c0d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0c0d-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0c0d-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0c0d-108">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="d0c0d-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="d0c0d-109">Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.</span><span class="sxs-lookup"><span data-stu-id="d0c0d-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="d0c0d-110">Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.</span><span class="sxs-lookup"><span data-stu-id="d0c0d-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="d0c0d-111">Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0c0d-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="d0c0d-112">Die folgenden Ressourcen: Grafik werden sowohl Intune Workflows verwendet:</span><span class="sxs-lookup"><span data-stu-id="d0c0d-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="d0c0d-113">Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="d0c0d-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="d0c0d-114">allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0c0d-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="d0c0d-115">allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0c0d-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="d0c0d-116">Compliance-status</span><span class="sxs-lookup"><span data-stu-id="d0c0d-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="d0c0d-117">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0c0d-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="d0c0d-118">Geräte-App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="d0c0d-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="d0c0d-119">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="d0c0d-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="d0c0d-120">Registrierung Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="d0c0d-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="d0c0d-121">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d0c0d-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="d0c0d-122">Gerätetyp-Plattform</span><span class="sxs-lookup"><span data-stu-id="d0c0d-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="d0c0d-123">Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="d0c0d-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="d0c0d-124">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="d0c0d-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="d0c0d-125">exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0c0d-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="d0c0d-126">groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0c0d-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="d0c0d-127">Installieren Sie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="d0c0d-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="d0c0d-128">ipRange</span><span class="sxs-lookup"><span data-stu-id="d0c0d-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="d0c0d-129">iPv4Range</span><span class="sxs-lookup"><span data-stu-id="d0c0d-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="d0c0d-130">iPv6Range</span><span class="sxs-lookup"><span data-stu-id="d0c0d-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="d0c0d-131">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="d0c0d-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="d0c0d-132">MIME-Inhalt</span><span class="sxs-lookup"><span data-stu-id="d0c0d-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="d0c0d-133">proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="d0c0d-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="d0c0d-134">Report</span><span class="sxs-lookup"><span data-stu-id="d0c0d-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="d0c0d-135">reportRoot</span><span class="sxs-lookup"><span data-stu-id="d0c0d-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="d0c0d-136">Resultierende app-Status</span><span class="sxs-lookup"><span data-stu-id="d0c0d-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="d0c0d-137">RGB-Farbe</span><span class="sxs-lookup"><span data-stu-id="d0c0d-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="d0c0d-138">Führen Sie als Kontotyp</span><span class="sxs-lookup"><span data-stu-id="d0c0d-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="d0c0d-139">Führen Sie Zustand</span><span class="sxs-lookup"><span data-stu-id="d0c0d-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="d0c0d-140">Gespeichert von Benutzeroberflächenoptionen Zustand-Generierung</span><span class="sxs-lookup"><span data-stu-id="d0c0d-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="d0c0d-141">URI</span><span class="sxs-lookup"><span data-stu-id="d0c0d-141">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="d0c0d-142">Benutzer</span><span class="sxs-lookup"><span data-stu-id="d0c0d-142">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="d0c0d-143">VPP token Kontotyp</span><span class="sxs-lookup"><span data-stu-id="d0c0d-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="d0c0d-144">VPP token Aktion Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="d0c0d-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="d0c0d-145">Windows-Domäne Join-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d0c0d-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
