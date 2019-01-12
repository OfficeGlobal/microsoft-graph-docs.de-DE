---
title: DeviceEnrollmentType Enum-Typ
description: Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987755"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="fc880-103">DeviceEnrollmentType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fc880-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="fc880-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc880-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc880-105">Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.</span><span class="sxs-lookup"><span data-stu-id="fc880-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="fc880-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="fc880-106">Members</span></span>
|<span data-ttu-id="fc880-107">Element</span><span class="sxs-lookup"><span data-stu-id="fc880-107">Member</span></span>|<span data-ttu-id="fc880-108">Wert</span><span class="sxs-lookup"><span data-stu-id="fc880-108">Value</span></span>|<span data-ttu-id="fc880-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc880-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc880-110">unknown</span><span class="sxs-lookup"><span data-stu-id="fc880-110">unknown</span></span>|<span data-ttu-id="fc880-111">0</span><span class="sxs-lookup"><span data-stu-id="fc880-111">0</span></span>|<span data-ttu-id="fc880-112">Standardwert, Registrierung Typ wurde nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="fc880-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="fc880-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="fc880-113">userEnrollment</span></span>|<span data-ttu-id="fc880-114">1</span><span class="sxs-lookup"><span data-stu-id="fc880-114">1</span></span>|<span data-ttu-id="fc880-115">Benutzer gesteuerten Registrierung über BYOD Kanal.</span><span class="sxs-lookup"><span data-stu-id="fc880-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="fc880-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="fc880-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="fc880-117">2</span><span class="sxs-lookup"><span data-stu-id="fc880-117">2</span></span>|<span data-ttu-id="fc880-118">Registrierung der Benutzer mit einem Gerät Registrierungs-Manager-Konto.</span><span class="sxs-lookup"><span data-stu-id="fc880-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="fc880-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="fc880-119">appleBulkWithUser</span></span>|<span data-ttu-id="fc880-120">3</span><span class="sxs-lookup"><span data-stu-id="fc880-120">3</span></span>|<span data-ttu-id="fc880-121">Apple Bulk Registrierung mit dem Benutzer Herausforderung (DEP, Apple-Konfiguration).</span><span class="sxs-lookup"><span data-stu-id="fc880-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="fc880-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="fc880-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="fc880-123">4</span><span class="sxs-lookup"><span data-stu-id="fc880-123">4</span></span>|<span data-ttu-id="fc880-124">Apple Bulk Registrierung ohne Benutzer Herausforderung (DEP Apple-Konfiguration, Mobile Config).</span><span class="sxs-lookup"><span data-stu-id="fc880-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="fc880-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="fc880-125">windowsAzureADJoin</span></span>|<span data-ttu-id="fc880-126">5</span><span class="sxs-lookup"><span data-stu-id="fc880-126">5</span></span>|<span data-ttu-id="fc880-127">Windows Azure AD 10 teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="fc880-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="fc880-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="fc880-128">windowsBulkUserless</span></span>|<span data-ttu-id="fc880-129">6</span><span class="sxs-lookup"><span data-stu-id="fc880-129">6</span></span>|<span data-ttu-id="fc880-130">Windows 10 Bulk Registrierung über ICD mit dem Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="fc880-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="fc880-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="fc880-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="fc880-132">7</span><span class="sxs-lookup"><span data-stu-id="fc880-132">7</span></span>|<span data-ttu-id="fc880-133">Automatische 10 Windows-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="fc880-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="fc880-134">(Arbeit Konto hinzufügen)</span><span class="sxs-lookup"><span data-stu-id="fc880-134">(Add work account)</span></span>|
|<span data-ttu-id="fc880-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="fc880-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="fc880-136">8</span><span class="sxs-lookup"><span data-stu-id="fc880-136">8</span></span>|<span data-ttu-id="fc880-137">Massen-10 Windows Azure AD teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="fc880-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="fc880-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="fc880-138">windowsCoManagement</span></span>|<span data-ttu-id="fc880-139">9</span><span class="sxs-lookup"><span data-stu-id="fc880-139">9</span></span>|<span data-ttu-id="fc880-140">Windows 10 gemeinsame Verwaltung durch AutoPilot oder Gruppenrichtlinien ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="fc880-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



