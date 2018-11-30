---
title: Gemeinsam genutzten Ressourcen in Microsoft Intune
description: Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.  Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.  Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.
ms.openlocfilehash: 8355d3b4bcb9b4fdc7fc8c1874641117dad1d583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019986"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="42bad-105">Gemeinsam genutzten Ressourcen in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="42bad-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="42bad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="42bad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="42bad-107">Diese Endpunkte werden in mehreren Microsoft Graph-API für Intune Workflows verwendet.</span><span class="sxs-lookup"><span data-stu-id="42bad-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="42bad-108">Die Absicht, den Zweck und die erforderlichen Berechtigungen für eine bestimmte Ressource verwenden variiert je nach den bestimmten Workflow und dem Kontext des zugrunde liegenden Anrufs.</span><span class="sxs-lookup"><span data-stu-id="42bad-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="42bad-109">Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="42bad-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="42bad-110">Die folgenden Ressourcen: Grafik werden sowohl Intune Workflows verwendet:</span><span class="sxs-lookup"><span data-stu-id="42bad-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="42bad-111">allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42bad-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="42bad-112">allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42bad-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="42bad-113">Compliance-status</span><span class="sxs-lookup"><span data-stu-id="42bad-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="42bad-114">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42bad-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="42bad-115">Geräte-App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="42bad-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="42bad-116">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="42bad-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="42bad-117">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="42bad-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="42bad-118">exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42bad-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="42bad-119">groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42bad-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="42bad-120">Installieren Sie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="42bad-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="42bad-121">MIME-Inhalt</span><span class="sxs-lookup"><span data-stu-id="42bad-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="42bad-122">Report</span><span class="sxs-lookup"><span data-stu-id="42bad-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="42bad-123">reportRoot</span><span class="sxs-lookup"><span data-stu-id="42bad-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="42bad-124">Gespeichert von Benutzeroberflächenoptionen Zustand-Generierung</span><span class="sxs-lookup"><span data-stu-id="42bad-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="42bad-125">URI</span><span class="sxs-lookup"><span data-stu-id="42bad-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="42bad-126">User</span><span class="sxs-lookup"><span data-stu-id="42bad-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="42bad-127">VPP token Kontotyp</span><span class="sxs-lookup"><span data-stu-id="42bad-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
