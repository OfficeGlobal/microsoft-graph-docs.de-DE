---
title: deviceEnrollmentType-Enumerationstyp
description: Mögliche Möglichkeiten zum Hinzufügen eines mobilen Geräts zur Verwaltung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62ff257e2f758776265f52a0d64cde52dbc26115
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261964"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="4550c-103">deviceEnrollmentType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="4550c-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="4550c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4550c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4550c-105">Mögliche Möglichkeiten zum Hinzufügen eines mobilen Geräts zur Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="4550c-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="4550c-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="4550c-106">Members</span></span>
|<span data-ttu-id="4550c-107">Element</span><span class="sxs-lookup"><span data-stu-id="4550c-107">Member</span></span>|<span data-ttu-id="4550c-108">Wert</span><span class="sxs-lookup"><span data-stu-id="4550c-108">Value</span></span>|<span data-ttu-id="4550c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4550c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4550c-110">unknown</span><span class="sxs-lookup"><span data-stu-id="4550c-110">unknown</span></span>|<span data-ttu-id="4550c-111">0</span><span class="sxs-lookup"><span data-stu-id="4550c-111">0</span></span>|<span data-ttu-id="4550c-112">Standardwert, der Registrierungstyp wurde nicht gesammelt.</span><span class="sxs-lookup"><span data-stu-id="4550c-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="4550c-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="4550c-113">userEnrollment</span></span>|<span data-ttu-id="4550c-114">1</span><span class="sxs-lookup"><span data-stu-id="4550c-114">1</span></span>|<span data-ttu-id="4550c-115">Benutzergesteuerte Registrierung über den BYOD-Kanal.</span><span class="sxs-lookup"><span data-stu-id="4550c-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="4550c-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="4550c-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="4550c-117">2</span><span class="sxs-lookup"><span data-stu-id="4550c-117">2</span></span>|<span data-ttu-id="4550c-118">Benutzerregistrierung mit einem Geräte Registrierungs-Manager-Konto.</span><span class="sxs-lookup"><span data-stu-id="4550c-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="4550c-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="4550c-119">appleBulkWithUser</span></span>|<span data-ttu-id="4550c-120">3</span><span class="sxs-lookup"><span data-stu-id="4550c-120">3</span></span>|<span data-ttu-id="4550c-121">Apple Bulk Enrollment with User Challenge.</span><span class="sxs-lookup"><span data-stu-id="4550c-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="4550c-122">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="4550c-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="4550c-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="4550c-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="4550c-124">4</span><span class="sxs-lookup"><span data-stu-id="4550c-124">4</span></span>|<span data-ttu-id="4550c-125">Apple-Massenregistrierung ohne Benutzer Herausforderung.</span><span class="sxs-lookup"><span data-stu-id="4550c-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="4550c-126">(DEP, Apple Configurator, Mobile Konfiguration)</span><span class="sxs-lookup"><span data-stu-id="4550c-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="4550c-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="4550c-127">windowsAzureADJoin</span></span>|<span data-ttu-id="4550c-128">5</span><span class="sxs-lookup"><span data-stu-id="4550c-128">5</span></span>|<span data-ttu-id="4550c-129">Windows 10 Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="4550c-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="4550c-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="4550c-130">windowsBulkUserless</span></span>|<span data-ttu-id="4550c-131">6</span><span class="sxs-lookup"><span data-stu-id="4550c-131">6</span></span>|<span data-ttu-id="4550c-132">Windows 10 Bulk-Registrierung über ICD mit Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="4550c-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="4550c-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="4550c-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="4550c-134">7</span><span class="sxs-lookup"><span data-stu-id="4550c-134">7</span></span>|<span data-ttu-id="4550c-135">Automatische Windows 10-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="4550c-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="4550c-136">(Arbeitskonto hinzufügen)</span><span class="sxs-lookup"><span data-stu-id="4550c-136">(Add work account)</span></span>|
|<span data-ttu-id="4550c-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="4550c-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="4550c-138">8</span><span class="sxs-lookup"><span data-stu-id="4550c-138">8</span></span>|<span data-ttu-id="4550c-139">Windows 10 Bulk Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="4550c-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="4550c-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="4550c-140">windowsCoManagement</span></span>|<span data-ttu-id="4550c-141">9</span><span class="sxs-lookup"><span data-stu-id="4550c-141">9</span></span>|<span data-ttu-id="4550c-142">Durch autoPilot oder Gruppenrichtlinien ausgelöste Windows 10-Co-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="4550c-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



