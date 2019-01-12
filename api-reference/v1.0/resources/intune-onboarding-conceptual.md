---
title: Registrieren von Geräten für die Verwaltung in Intune
description: " Registrierung (BYOD) kann Benutzer ihre persönliche Telefone, Tablets oder PCs zu registrieren. Die Registrierung unternehmenseigener Geräte (COD) ermöglicht Verwaltungsszenarien wie Remotezurücksetzung, gemeinsam genutzte Geräte oder Benutzeraffinität für ein Gerät."
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2e7f6e85e32137804556c64a1995bd2e78b04068
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917440"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="5a04a-104">Registrieren von Geräten für die Verwaltung in Intune</span><span class="sxs-lookup"><span data-stu-id="5a04a-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="5a04a-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="5a04a-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="5a04a-106">Sie können Geräte wie z. B. Windows-PCs registrieren, um die Verwaltung mobiler Geräte (MDM) mit Microsoft Intune zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5a04a-106">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="5a04a-107">In diesem Thema werden verschiedene Methoden für die Registrierung mobiler Geräte für die Verwaltung in Intune beschrieben.</span><span class="sxs-lookup"><span data-stu-id="5a04a-107">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="5a04a-108">Die Art der Registrierung hängt vom Gerätetyp, der Eigentümerschaft und dem erforderlichen Verwaltungsgrad ab.</span><span class="sxs-lookup"><span data-stu-id="5a04a-108">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="5a04a-109">Bei der „Bring your own device“ (BYOD)-Registrierung können Benutzer ihre eigenen Smartphones, Tablets oder PCs registrieren.</span><span class="sxs-lookup"><span data-stu-id="5a04a-109">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="5a04a-110">Die Registrierung unternehmenseigener Geräte (COD) ermöglicht Verwaltungsszenarien wie Remotezurücksetzung, gemeinsam genutzte Geräte oder Benutzeraffinität für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="5a04a-110">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="5a04a-111">Die folgenden Graph-Ressourcen stehen für die Registrierungsverwaltung in Intune zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="5a04a-111">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="5a04a-112">Konfiguration der Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="5a04a-112">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="5a04a-113">Konfiguration der Geräteregistrierungsgrenze</span><span class="sxs-lookup"><span data-stu-id="5a04a-113">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="5a04a-114">Geräteregistrierung – Plattformeinschränkung</span><span class="sxs-lookup"><span data-stu-id="5a04a-114">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="5a04a-115">Konfiguration der Plattformeinschränkungen für Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="5a04a-115">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="5a04a-116">Geräteregistrierung – Windows Hello für Business-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="5a04a-116">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="5a04a-117">Exchange Connector für Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="5a04a-117">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="5a04a-118">Verwaltung von Exchange Connector Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="5a04a-118">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="5a04a-119">Verwaltung von Exchange Connector Sync Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="5a04a-119">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="5a04a-120">Verwaltung von Exchange Connector Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="5a04a-120">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="5a04a-121">Geräteverwaltungspartner</span><span class="sxs-lookup"><span data-stu-id="5a04a-121">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="5a04a-122">Gerät Management Partner app-Typ</span><span class="sxs-lookup"><span data-stu-id="5a04a-122">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="5a04a-123">Management Partner Mandanten Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="5a04a-123">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="5a04a-124">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="5a04a-124">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="5a04a-125">Zuweisung der Registrierungskonfiguration</span><span class="sxs-lookup"><span data-stu-id="5a04a-125">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="5a04a-126">Intune-Marke</span><span class="sxs-lookup"><span data-stu-id="5a04a-126">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="5a04a-127">MDM Autorität</span><span class="sxs-lookup"><span data-stu-id="5a04a-127">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="5a04a-128">MTD-Connector (Mobile Threat Defense)</span><span class="sxs-lookup"><span data-stu-id="5a04a-128">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="5a04a-129">Mobile Bedrohung Partner Mandanten Zustand</span><span class="sxs-lookup"><span data-stu-id="5a04a-129">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="5a04a-130">Einstellungen für lokalen, bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="5a04a-130">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="5a04a-131">Organisation</span><span class="sxs-lookup"><span data-stu-id="5a04a-131">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="5a04a-132">RGB-Farbe</span><span class="sxs-lookup"><span data-stu-id="5a04a-132">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="5a04a-133">VPP token</span><span class="sxs-lookup"><span data-stu-id="5a04a-133">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="5a04a-134">VPP token Zustand</span><span class="sxs-lookup"><span data-stu-id="5a04a-134">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="5a04a-135">VPP token Synchronisierungsstatus</span><span class="sxs-lookup"><span data-stu-id="5a04a-135">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="5a04a-136">Windows Hello für die Verwendung der Business-PIN</span><span class="sxs-lookup"><span data-stu-id="5a04a-136">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
