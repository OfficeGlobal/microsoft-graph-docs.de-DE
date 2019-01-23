---
title: Gemeinsam genutzten Ressourcen in Microsoft Intune
description: Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.  Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.  Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 11ee529edd3d74b5d6fb0c2d9d4e63bada0b0b22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415432"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="d456a-105">Gemeinsam genutzten Ressourcen in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d456a-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="d456a-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d456a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d456a-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d456a-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d456a-108">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="d456a-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="d456a-109">Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.</span><span class="sxs-lookup"><span data-stu-id="d456a-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="d456a-110">Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.</span><span class="sxs-lookup"><span data-stu-id="d456a-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="d456a-111">Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d456a-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="d456a-112">Die folgenden Ressourcen: Grafik werden sowohl Intune Workflows verwendet:</span><span class="sxs-lookup"><span data-stu-id="d456a-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="d456a-113">Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="d456a-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="d456a-114">allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d456a-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="d456a-115">allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d456a-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="d456a-116">Compliance-status</span><span class="sxs-lookup"><span data-stu-id="d456a-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="d456a-117">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d456a-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="d456a-118">Geräte-App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="d456a-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="d456a-119">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="d456a-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="d456a-120">Registrierung Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="d456a-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="d456a-121">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d456a-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="d456a-122">Gerätetyp-Plattform</span><span class="sxs-lookup"><span data-stu-id="d456a-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="d456a-123">Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="d456a-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="d456a-124">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="d456a-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="d456a-125">exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d456a-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="d456a-126">groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d456a-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="d456a-127">Installieren Sie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="d456a-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="d456a-128">ipRange</span><span class="sxs-lookup"><span data-stu-id="d456a-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="d456a-129">iPv4Range</span><span class="sxs-lookup"><span data-stu-id="d456a-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="d456a-130">iPv6Range</span><span class="sxs-lookup"><span data-stu-id="d456a-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="d456a-131">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="d456a-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="d456a-132">MIME-Inhalt</span><span class="sxs-lookup"><span data-stu-id="d456a-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="d456a-133">Problembehandlung bei mobilen app-Ereignis</span><span class="sxs-lookup"><span data-stu-id="d456a-133">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="d456a-134">proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="d456a-134">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="d456a-135">Report</span><span class="sxs-lookup"><span data-stu-id="d456a-135">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="d456a-136">reportRoot</span><span class="sxs-lookup"><span data-stu-id="d456a-136">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="d456a-137">Resultierende app-Status</span><span class="sxs-lookup"><span data-stu-id="d456a-137">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="d456a-138">RGB-Farbe</span><span class="sxs-lookup"><span data-stu-id="d456a-138">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="d456a-139">Führen Sie als Kontotyp</span><span class="sxs-lookup"><span data-stu-id="d456a-139">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="d456a-140">Führen Sie Zustand</span><span class="sxs-lookup"><span data-stu-id="d456a-140">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="d456a-141">Gespeichert von Benutzeroberflächenoptionen Zustand-Generierung</span><span class="sxs-lookup"><span data-stu-id="d456a-141">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="d456a-142">URI</span><span class="sxs-lookup"><span data-stu-id="d456a-142">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="d456a-143">Benutzer</span><span class="sxs-lookup"><span data-stu-id="d456a-143">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="d456a-144">VPP token Kontotyp</span><span class="sxs-lookup"><span data-stu-id="d456a-144">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="d456a-145">VPP token Aktion Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="d456a-145">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="d456a-146">Windows-Domäne Join-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d456a-146">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
