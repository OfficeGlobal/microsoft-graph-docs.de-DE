---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67dd3850db1e759ded578f551eb41636ec231084
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985963"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="ebbaa-103">EmbeddedSIMDeviceStateValue Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ebbaa-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="ebbaa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebbaa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebbaa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebbaa-107">Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="ebbaa-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="ebbaa-108">Members</span></span>
|<span data-ttu-id="ebbaa-109">Element</span><span class="sxs-lookup"><span data-stu-id="ebbaa-109">Member</span></span>|<span data-ttu-id="ebbaa-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ebbaa-110">Value</span></span>|<span data-ttu-id="ebbaa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebbaa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbaa-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="ebbaa-112">notEvaluated</span></span>|<span data-ttu-id="ebbaa-113">0</span><span class="sxs-lookup"><span data-stu-id="ebbaa-113">0</span></span>|<span data-ttu-id="ebbaa-114">Legt fest, dass der eingebettete SIM Aktivierungscode kostenlosen und verfügbar ist, ein Gerät zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="ebbaa-115">failed</span><span class="sxs-lookup"><span data-stu-id="ebbaa-115">failed</span></span>|<span data-ttu-id="ebbaa-116">1</span><span class="sxs-lookup"><span data-stu-id="ebbaa-116">1</span></span>|<span data-ttu-id="ebbaa-117">Legt fest, dass Intune Service konnte nicht an einem Gerät dieses Profil übermitteln.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="ebbaa-118">Installieren von</span><span class="sxs-lookup"><span data-stu-id="ebbaa-118">installing</span></span>|<span data-ttu-id="ebbaa-119">2</span><span class="sxs-lookup"><span data-stu-id="ebbaa-119">2</span></span>|<span data-ttu-id="ebbaa-120">Legt fest, dass der eingebettete SIM Aktivierungscode zu einem Gerät zugewiesen wurde, und das Gerät wird das Token installieren.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="ebbaa-121">installiert</span><span class="sxs-lookup"><span data-stu-id="ebbaa-121">installed</span></span>|<span data-ttu-id="ebbaa-122">3</span><span class="sxs-lookup"><span data-stu-id="ebbaa-122">3</span></span>|<span data-ttu-id="ebbaa-123">Legt fest, dass der eingebettete SIM Aktivierungscode auf das Zielgerät erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="ebbaa-124">Löschen</span><span class="sxs-lookup"><span data-stu-id="ebbaa-124">deleting</span></span>|<span data-ttu-id="ebbaa-125">4</span><span class="sxs-lookup"><span data-stu-id="ebbaa-125">4</span></span>|<span data-ttu-id="ebbaa-126">Legt fest, dass Intune Service versucht, um das Profil vom Gerät zu löschen.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="ebbaa-127">error</span><span class="sxs-lookup"><span data-stu-id="ebbaa-127">error</span></span>|<span data-ttu-id="ebbaa-128">5</span><span class="sxs-lookup"><span data-stu-id="ebbaa-128">5</span></span>|<span data-ttu-id="ebbaa-129">Legt fest, dass Fehler mit diesem Profil vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="ebbaa-130">gelöscht</span><span class="sxs-lookup"><span data-stu-id="ebbaa-130">deleted</span></span>|<span data-ttu-id="ebbaa-131">6</span><span class="sxs-lookup"><span data-stu-id="ebbaa-131">6</span></span>|<span data-ttu-id="ebbaa-132">Legt fest, dass das Profil vom Gerät gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="ebbaa-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="ebbaa-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="ebbaa-133">removedByUser</span></span>|<span data-ttu-id="ebbaa-134">7</span><span class="sxs-lookup"><span data-stu-id="ebbaa-134">7</span></span>|<span data-ttu-id="ebbaa-135">Legt fest, dass das Profil des Benutzers vom Gerät entfernt wird</span><span class="sxs-lookup"><span data-stu-id="ebbaa-135">Designates that the profile is removed from the device by the user</span></span>|





