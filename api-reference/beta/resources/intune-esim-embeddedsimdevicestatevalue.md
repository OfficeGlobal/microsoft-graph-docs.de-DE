---
title: embeddedSIMDeviceStateValue-Enumerationstyp
description: Beschreibt die verschiedenen Status für einen eingebetteten SIM-Aktivierungscode.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bdc3250605de7db7a3778d64b5e743a415de4c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145423"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="8e1bb-103">embeddedSIMDeviceStateValue-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="8e1bb-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="8e1bb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e1bb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e1bb-106">Beschreibt die verschiedenen Status für einen eingebetteten SIM-Aktivierungscode.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="8e1bb-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="8e1bb-107">Members</span></span>
|<span data-ttu-id="8e1bb-108">Element</span><span class="sxs-lookup"><span data-stu-id="8e1bb-108">Member</span></span>|<span data-ttu-id="8e1bb-109">Wert</span><span class="sxs-lookup"><span data-stu-id="8e1bb-109">Value</span></span>|<span data-ttu-id="8e1bb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e1bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e1bb-111">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="8e1bb-111">notEvaluated</span></span>|<span data-ttu-id="8e1bb-112">0</span><span class="sxs-lookup"><span data-stu-id="8e1bb-112">0</span></span>|<span data-ttu-id="8e1bb-113">Gibt an, dass der eingebettete SIM-Aktivierungscode kostenlos ist und einem Gerät zugewiesen werden kann.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="8e1bb-114">failed</span><span class="sxs-lookup"><span data-stu-id="8e1bb-114">failed</span></span>|<span data-ttu-id="8e1bb-115">1</span><span class="sxs-lookup"><span data-stu-id="8e1bb-115">1</span></span>|<span data-ttu-id="8e1bb-116">Gibt an, dass InTune-Dienst dieses Profil nicht an ein Gerät übermitteln konnte.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="8e1bb-117">Installieren</span><span class="sxs-lookup"><span data-stu-id="8e1bb-117">installing</span></span>|<span data-ttu-id="8e1bb-118">2</span><span class="sxs-lookup"><span data-stu-id="8e1bb-118">2</span></span>|<span data-ttu-id="8e1bb-119">Gibt an, dass der eingebettete SIM-Aktivierungscode einem Gerät zugewiesen wurde und das Gerät das Token installiert.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="8e1bb-120">installiert</span><span class="sxs-lookup"><span data-stu-id="8e1bb-120">installed</span></span>|<span data-ttu-id="8e1bb-121">3</span><span class="sxs-lookup"><span data-stu-id="8e1bb-121">3</span></span>|<span data-ttu-id="8e1bb-122">Gibt an, dass der eingebettete SIM-Aktivierungscode erfolgreich auf dem Zielgerät installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="8e1bb-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="8e1bb-123">deleting</span></span>|<span data-ttu-id="8e1bb-124">4</span><span class="sxs-lookup"><span data-stu-id="8e1bb-124">4</span></span>|<span data-ttu-id="8e1bb-125">Gibt an, dass InTune-Dienst versucht, das Profil vom Gerät zu löschen.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="8e1bb-126">error</span><span class="sxs-lookup"><span data-stu-id="8e1bb-126">error</span></span>|<span data-ttu-id="8e1bb-127">5</span><span class="sxs-lookup"><span data-stu-id="8e1bb-127">5</span></span>|<span data-ttu-id="8e1bb-128">Gibt an, dass ein Fehler mit diesem Profil vorliegt.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="8e1bb-129">deleted</span><span class="sxs-lookup"><span data-stu-id="8e1bb-129">deleted</span></span>|<span data-ttu-id="8e1bb-130">6</span><span class="sxs-lookup"><span data-stu-id="8e1bb-130">6</span></span>|<span data-ttu-id="8e1bb-131">Legt fest, dass das Profil vom Gerät gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="8e1bb-132">removedByUser</span><span class="sxs-lookup"><span data-stu-id="8e1bb-132">removedByUser</span></span>|<span data-ttu-id="8e1bb-133">7</span><span class="sxs-lookup"><span data-stu-id="8e1bb-133">7</span></span>|<span data-ttu-id="8e1bb-134">Legt fest, dass das Profil vom Benutzer vom Gerät entfernt wurde.</span><span class="sxs-lookup"><span data-stu-id="8e1bb-134">Designates that the profile is removed from the device by the user</span></span>|




