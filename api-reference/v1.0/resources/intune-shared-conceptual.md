---
title: Gemeinsam genutzten Ressourcen in Microsoft Intune
description: Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.  Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.  Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.
localization_priority: Normal
ms.openlocfilehash: d0d615be8d185c5dfe24d58f6a2e371e6baf18c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840068"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="7c054-105">Gemeinsam genutzten Ressourcen in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7c054-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="7c054-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="7c054-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="7c054-107">Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.</span><span class="sxs-lookup"><span data-stu-id="7c054-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="7c054-108">Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.</span><span class="sxs-lookup"><span data-stu-id="7c054-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="7c054-109">Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c054-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="7c054-110">Die folgenden Ressourcen: Grafik werden sowohl Intune Workflows verwendet:</span><span class="sxs-lookup"><span data-stu-id="7c054-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="7c054-111">allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c054-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="7c054-112">allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c054-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="7c054-113">Compliance-status</span><span class="sxs-lookup"><span data-stu-id="7c054-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="7c054-114">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c054-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="7c054-115">Geräte-App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="7c054-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="7c054-116">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="7c054-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="7c054-117">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7c054-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="7c054-118">exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c054-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="7c054-119">groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c054-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="7c054-120">Installieren Sie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="7c054-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="7c054-121">MIME-Inhalt</span><span class="sxs-lookup"><span data-stu-id="7c054-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="7c054-122">Report</span><span class="sxs-lookup"><span data-stu-id="7c054-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="7c054-123">reportRoot</span><span class="sxs-lookup"><span data-stu-id="7c054-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="7c054-124">Gespeichert von Benutzeroberflächenoptionen Zustand-Generierung</span><span class="sxs-lookup"><span data-stu-id="7c054-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="7c054-125">URI</span><span class="sxs-lookup"><span data-stu-id="7c054-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="7c054-126">Benutzer</span><span class="sxs-lookup"><span data-stu-id="7c054-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="7c054-127">VPP token Kontotyp</span><span class="sxs-lookup"><span data-stu-id="7c054-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
