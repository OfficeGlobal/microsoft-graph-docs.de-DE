---
title: deviceEnrollmentType-Enumerationstyp
description: Mögliche Möglichkeiten zum Hinzufügen eines mobilen Geräts zur Verwaltung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173654"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="e8d8a-103">deviceEnrollmentType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="e8d8a-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="e8d8a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8d8a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8d8a-106">Mögliche Möglichkeiten zum Hinzufügen eines mobilen Geräts zur Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="e8d8a-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="e8d8a-107">Members</span></span>
|<span data-ttu-id="e8d8a-108">Element</span><span class="sxs-lookup"><span data-stu-id="e8d8a-108">Member</span></span>|<span data-ttu-id="e8d8a-109">Wert</span><span class="sxs-lookup"><span data-stu-id="e8d8a-109">Value</span></span>|<span data-ttu-id="e8d8a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8d8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8d8a-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e8d8a-111">unknown</span></span>|<span data-ttu-id="e8d8a-112">0</span><span class="sxs-lookup"><span data-stu-id="e8d8a-112">0</span></span>|<span data-ttu-id="e8d8a-113">Standardwert, der Registrierungstyp wurde nicht gesammelt.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="e8d8a-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="e8d8a-114">userEnrollment</span></span>|<span data-ttu-id="e8d8a-115">1</span><span class="sxs-lookup"><span data-stu-id="e8d8a-115">1</span></span>|<span data-ttu-id="e8d8a-116">Benutzergesteuerte Registrierung über den BYOD-Kanal.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="e8d8a-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="e8d8a-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="e8d8a-118">2</span><span class="sxs-lookup"><span data-stu-id="e8d8a-118">2</span></span>|<span data-ttu-id="e8d8a-119">Benutzerregistrierung mit einem Geräte Registrierungs-Manager-Konto.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="e8d8a-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="e8d8a-120">appleBulkWithUser</span></span>|<span data-ttu-id="e8d8a-121">3</span><span class="sxs-lookup"><span data-stu-id="e8d8a-121">3</span></span>|<span data-ttu-id="e8d8a-122">Apple Bulk Enrollment with User Challenge.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="e8d8a-123">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="e8d8a-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="e8d8a-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="e8d8a-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="e8d8a-125">4</span><span class="sxs-lookup"><span data-stu-id="e8d8a-125">4</span></span>|<span data-ttu-id="e8d8a-126">Apple-Massenregistrierung ohne Benutzer Herausforderung.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="e8d8a-127">(DEP, Apple Configurator, Mobile Konfiguration)</span><span class="sxs-lookup"><span data-stu-id="e8d8a-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="e8d8a-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="e8d8a-128">windowsAzureADJoin</span></span>|<span data-ttu-id="e8d8a-129">5</span><span class="sxs-lookup"><span data-stu-id="e8d8a-129">5</span></span>|<span data-ttu-id="e8d8a-130">Windows 10 Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="e8d8a-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="e8d8a-131">windowsBulkUserless</span></span>|<span data-ttu-id="e8d8a-132">6</span><span class="sxs-lookup"><span data-stu-id="e8d8a-132">6</span></span>|<span data-ttu-id="e8d8a-133">Windows 10 Bulk-Registrierung über ICD mit Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="e8d8a-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="e8d8a-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="e8d8a-135">7</span><span class="sxs-lookup"><span data-stu-id="e8d8a-135">7</span></span>|<span data-ttu-id="e8d8a-136">Automatische Windows 10-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="e8d8a-137">(Arbeitskonto hinzufügen)</span><span class="sxs-lookup"><span data-stu-id="e8d8a-137">(Add work account)</span></span>|
|<span data-ttu-id="e8d8a-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="e8d8a-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="e8d8a-139">8</span><span class="sxs-lookup"><span data-stu-id="e8d8a-139">8</span></span>|<span data-ttu-id="e8d8a-140">Windows 10 Bulk Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="e8d8a-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="e8d8a-141">windowsCoManagement</span></span>|<span data-ttu-id="e8d8a-142">9</span><span class="sxs-lookup"><span data-stu-id="e8d8a-142">9</span></span>|<span data-ttu-id="e8d8a-143">Durch autoPilot oder Gruppenrichtlinien ausgelöste Windows 10-Co-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="e8d8a-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




