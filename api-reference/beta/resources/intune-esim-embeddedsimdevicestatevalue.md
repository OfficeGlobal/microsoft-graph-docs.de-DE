---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421326"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="474fe-103">EmbeddedSIMDeviceStateValue Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="474fe-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="474fe-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="474fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="474fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="474fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="474fe-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="474fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="474fe-107">Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.</span><span class="sxs-lookup"><span data-stu-id="474fe-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="474fe-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="474fe-108">Members</span></span>
|<span data-ttu-id="474fe-109">Member</span><span class="sxs-lookup"><span data-stu-id="474fe-109">Member</span></span>|<span data-ttu-id="474fe-110">Wert</span><span class="sxs-lookup"><span data-stu-id="474fe-110">Value</span></span>|<span data-ttu-id="474fe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="474fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="474fe-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="474fe-112">notEvaluated</span></span>|<span data-ttu-id="474fe-113">0</span><span class="sxs-lookup"><span data-stu-id="474fe-113">0</span></span>|<span data-ttu-id="474fe-114">Legt fest, dass der eingebettete SIM Aktivierungscode kostenlosen und verfügbar ist, ein Gerät zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="474fe-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="474fe-115">failed</span><span class="sxs-lookup"><span data-stu-id="474fe-115">failed</span></span>|<span data-ttu-id="474fe-116">1</span><span class="sxs-lookup"><span data-stu-id="474fe-116">1</span></span>|<span data-ttu-id="474fe-117">Legt fest, dass Intune Service konnte nicht an einem Gerät dieses Profil übermitteln.</span><span class="sxs-lookup"><span data-stu-id="474fe-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="474fe-118">Installieren von</span><span class="sxs-lookup"><span data-stu-id="474fe-118">installing</span></span>|<span data-ttu-id="474fe-119">2</span><span class="sxs-lookup"><span data-stu-id="474fe-119">2</span></span>|<span data-ttu-id="474fe-120">Legt fest, dass der eingebettete SIM Aktivierungscode zu einem Gerät zugewiesen wurde, und das Gerät wird das Token installieren.</span><span class="sxs-lookup"><span data-stu-id="474fe-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="474fe-121">installiert</span><span class="sxs-lookup"><span data-stu-id="474fe-121">installed</span></span>|<span data-ttu-id="474fe-122">3</span><span class="sxs-lookup"><span data-stu-id="474fe-122">3</span></span>|<span data-ttu-id="474fe-123">Legt fest, dass der eingebettete SIM Aktivierungscode auf das Zielgerät erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="474fe-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="474fe-124">Löschen</span><span class="sxs-lookup"><span data-stu-id="474fe-124">deleting</span></span>|<span data-ttu-id="474fe-125">4</span><span class="sxs-lookup"><span data-stu-id="474fe-125">4</span></span>|<span data-ttu-id="474fe-126">Legt fest, dass Intune Service versucht, um das Profil vom Gerät zu löschen.</span><span class="sxs-lookup"><span data-stu-id="474fe-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="474fe-127">error</span><span class="sxs-lookup"><span data-stu-id="474fe-127">error</span></span>|<span data-ttu-id="474fe-128">5</span><span class="sxs-lookup"><span data-stu-id="474fe-128">5</span></span>|<span data-ttu-id="474fe-129">Legt fest, dass Fehler mit diesem Profil vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="474fe-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="474fe-130">gelöscht</span><span class="sxs-lookup"><span data-stu-id="474fe-130">deleted</span></span>|<span data-ttu-id="474fe-131">6</span><span class="sxs-lookup"><span data-stu-id="474fe-131">6</span></span>|<span data-ttu-id="474fe-132">Legt fest, dass das Profil vom Gerät gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="474fe-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="474fe-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="474fe-133">removedByUser</span></span>|<span data-ttu-id="474fe-134">7</span><span class="sxs-lookup"><span data-stu-id="474fe-134">7</span></span>|<span data-ttu-id="474fe-135">Legt fest, dass das Profil des Benutzers vom Gerät entfernt wird</span><span class="sxs-lookup"><span data-stu-id="474fe-135">Designates that the profile is removed from the device by the user</span></span>|




