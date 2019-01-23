---
title: DeviceEnrollmentType Enum-Typ
description: Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399290"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="3b559-103">DeviceEnrollmentType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3b559-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="3b559-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3b559-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b559-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b559-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b559-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b559-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b559-107">Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.</span><span class="sxs-lookup"><span data-stu-id="3b559-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="3b559-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3b559-108">Members</span></span>
|<span data-ttu-id="3b559-109">Member</span><span class="sxs-lookup"><span data-stu-id="3b559-109">Member</span></span>|<span data-ttu-id="3b559-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3b559-110">Value</span></span>|<span data-ttu-id="3b559-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b559-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b559-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3b559-112">unknown</span></span>|<span data-ttu-id="3b559-113">0</span><span class="sxs-lookup"><span data-stu-id="3b559-113">0</span></span>|<span data-ttu-id="3b559-114">Standardwert, Registrierung Typ wurde nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="3b559-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="3b559-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="3b559-115">userEnrollment</span></span>|<span data-ttu-id="3b559-116">1</span><span class="sxs-lookup"><span data-stu-id="3b559-116">1</span></span>|<span data-ttu-id="3b559-117">Benutzer gesteuerten Registrierung über BYOD Kanal.</span><span class="sxs-lookup"><span data-stu-id="3b559-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="3b559-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="3b559-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="3b559-119">2</span><span class="sxs-lookup"><span data-stu-id="3b559-119">2</span></span>|<span data-ttu-id="3b559-120">Registrierung der Benutzer mit einem Gerät Registrierungs-Manager-Konto.</span><span class="sxs-lookup"><span data-stu-id="3b559-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="3b559-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="3b559-121">appleBulkWithUser</span></span>|<span data-ttu-id="3b559-122">3</span><span class="sxs-lookup"><span data-stu-id="3b559-122">3</span></span>|<span data-ttu-id="3b559-123">Apple Bulk Registrierung mit dem Benutzer Herausforderung.</span><span class="sxs-lookup"><span data-stu-id="3b559-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="3b559-124">(DEP, Apple-Konfiguration)</span><span class="sxs-lookup"><span data-stu-id="3b559-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="3b559-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="3b559-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="3b559-126">4</span><span class="sxs-lookup"><span data-stu-id="3b559-126">4</span></span>|<span data-ttu-id="3b559-127">Apple Bulk Registrierung ohne Benutzer Herausforderung.</span><span class="sxs-lookup"><span data-stu-id="3b559-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="3b559-128">(Mobile Config DEP Apple-Konfiguration)</span><span class="sxs-lookup"><span data-stu-id="3b559-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="3b559-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="3b559-129">windowsAzureADJoin</span></span>|<span data-ttu-id="3b559-130">5</span><span class="sxs-lookup"><span data-stu-id="3b559-130">5</span></span>|<span data-ttu-id="3b559-131">Windows Azure AD 10 teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="3b559-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="3b559-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="3b559-132">windowsBulkUserless</span></span>|<span data-ttu-id="3b559-133">6</span><span class="sxs-lookup"><span data-stu-id="3b559-133">6</span></span>|<span data-ttu-id="3b559-134">Windows 10 Bulk Registrierung über ICD mit dem Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="3b559-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="3b559-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="3b559-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="3b559-136">7</span><span class="sxs-lookup"><span data-stu-id="3b559-136">7</span></span>|<span data-ttu-id="3b559-137">Automatische 10 Windows-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="3b559-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="3b559-138">(Arbeit Konto hinzufügen)</span><span class="sxs-lookup"><span data-stu-id="3b559-138">(Add work account)</span></span>|
|<span data-ttu-id="3b559-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="3b559-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="3b559-140">8</span><span class="sxs-lookup"><span data-stu-id="3b559-140">8</span></span>|<span data-ttu-id="3b559-141">Massen-10 Windows Azure AD teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="3b559-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="3b559-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="3b559-142">windowsCoManagement</span></span>|<span data-ttu-id="3b559-143">9</span><span class="sxs-lookup"><span data-stu-id="3b559-143">9</span></span>|<span data-ttu-id="3b559-144">Windows 10 Co-Management durch AutoPilot oder Gruppenrichtlinien ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="3b559-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




