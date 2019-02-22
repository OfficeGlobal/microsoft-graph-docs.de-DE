---
title: FreigeGebene Ressourcen in Microsoft InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) auf, die mehrere Workflows für eine mandantenorganisation unterstützen.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6436f134ae9e95623b073f6e645f0737d45d540e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158310"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="f1441-103">FreigeGebene Ressourcen in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="f1441-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="f1441-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1441-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1441-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1441-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1441-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="f1441-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="f1441-107">Diese Endpunkte werden in mehreren Microsoft Graph-APIs für InTune-Workflows verwendet.</span><span class="sxs-lookup"><span data-stu-id="f1441-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="f1441-108">Die Absicht, der Zweck und die Berechtigungen, die für die Verwendung einer bestimmten Ressource erforderlich sind, hängen vom jeweiligen Workflow und Kontext des zugrunde liegenden Aufrufs ab.</span><span class="sxs-lookup"><span data-stu-id="f1441-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="f1441-109">Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1441-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="f1441-110">Die folgenden Graph-Ressourcen werden zwischen InTune-Workflows gemeinsam genutzt:</span><span class="sxs-lookup"><span data-stu-id="f1441-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="f1441-111">Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="f1441-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="f1441-112">allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1441-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="f1441-113">allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1441-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="f1441-114">Compliance-Status</span><span class="sxs-lookup"><span data-stu-id="f1441-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="f1441-115">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1441-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="f1441-116">Geräte-App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="f1441-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="f1441-117">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="f1441-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="f1441-118">Geräteregistrierungstyp</span><span class="sxs-lookup"><span data-stu-id="f1441-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="f1441-119">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f1441-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="f1441-120">Geräteplattformtyp</span><span class="sxs-lookup"><span data-stu-id="f1441-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="f1441-121">Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="f1441-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="f1441-122">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1441-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="f1441-123">exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1441-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="f1441-124">groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1441-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="f1441-125">Installationsabsicht</span><span class="sxs-lookup"><span data-stu-id="f1441-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="f1441-126">ipRange</span><span class="sxs-lookup"><span data-stu-id="f1441-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="f1441-127">iPv4Range</span><span class="sxs-lookup"><span data-stu-id="f1441-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="f1441-128">iPv6Range</span><span class="sxs-lookup"><span data-stu-id="f1441-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="f1441-129">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="f1441-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="f1441-130">MIME-Inhalt</span><span class="sxs-lookup"><span data-stu-id="f1441-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="f1441-131">Mobile App – Problembehandlung – Ereignis</span><span class="sxs-lookup"><span data-stu-id="f1441-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="f1441-132">proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="f1441-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="f1441-133">Report</span><span class="sxs-lookup"><span data-stu-id="f1441-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="f1441-134">reportRoot</span><span class="sxs-lookup"><span data-stu-id="f1441-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="f1441-135">Resultierender App-Status</span><span class="sxs-lookup"><span data-stu-id="f1441-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="f1441-136">RGB-Farbe</span><span class="sxs-lookup"><span data-stu-id="f1441-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="f1441-137">Kontotyp „Ausführen als“</span><span class="sxs-lookup"><span data-stu-id="f1441-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="f1441-138">Ausführungsstatus</span><span class="sxs-lookup"><span data-stu-id="f1441-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="f1441-139">Gespeicherte Optionen für Generierung des Benutzeroberflächenzustands</span><span class="sxs-lookup"><span data-stu-id="f1441-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="f1441-140">URI</span><span class="sxs-lookup"><span data-stu-id="f1441-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="f1441-141">Benutzer</span><span class="sxs-lookup"><span data-stu-id="f1441-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="f1441-142">Kontotyp des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="f1441-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="f1441-143">Fehlerursache für VPP-Tokenaktion</span><span class="sxs-lookup"><span data-stu-id="f1441-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="f1441-144">Konfiguration für Windows-Domänenbeitritt</span><span class="sxs-lookup"><span data-stu-id="f1441-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
