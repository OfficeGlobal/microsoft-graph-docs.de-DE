---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
author: tfitzmac
ms.openlocfilehash: 51e550669d9cd29d7d5bb246fe2cba017b02187c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320594"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="33d14-103">EmbeddedSIMDeviceStateValue Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="33d14-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="33d14-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33d14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33d14-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33d14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33d14-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33d14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33d14-107">Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.</span><span class="sxs-lookup"><span data-stu-id="33d14-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="33d14-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="33d14-108">Members</span></span>
|<span data-ttu-id="33d14-109">Member</span><span class="sxs-lookup"><span data-stu-id="33d14-109">Member</span></span>|<span data-ttu-id="33d14-110">Wert</span><span class="sxs-lookup"><span data-stu-id="33d14-110">Value</span></span>|<span data-ttu-id="33d14-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33d14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33d14-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="33d14-112">notEvaluated</span></span>|<span data-ttu-id="33d14-113">0</span><span class="sxs-lookup"><span data-stu-id="33d14-113">0</span></span>|<span data-ttu-id="33d14-114">Legt fest, dass der eingebettete SIM Aktivierungscode kostenlosen und verfügbar ist, ein Gerät zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="33d14-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="33d14-115">failed</span><span class="sxs-lookup"><span data-stu-id="33d14-115">failed</span></span>|<span data-ttu-id="33d14-116">1</span><span class="sxs-lookup"><span data-stu-id="33d14-116">1</span></span>|<span data-ttu-id="33d14-117">Legt fest, dass Intune Service konnte nicht an einem Gerät dieses Profil übermitteln.</span><span class="sxs-lookup"><span data-stu-id="33d14-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="33d14-118">Installieren von</span><span class="sxs-lookup"><span data-stu-id="33d14-118">installing</span></span>|<span data-ttu-id="33d14-119">2</span><span class="sxs-lookup"><span data-stu-id="33d14-119">2</span></span>|<span data-ttu-id="33d14-120">Legt fest, dass der eingebettete SIM Aktivierungscode zu einem Gerät zugewiesen wurde, und das Gerät wird das Token installieren.</span><span class="sxs-lookup"><span data-stu-id="33d14-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="33d14-121">installiert</span><span class="sxs-lookup"><span data-stu-id="33d14-121">installed</span></span>|<span data-ttu-id="33d14-122">3</span><span class="sxs-lookup"><span data-stu-id="33d14-122">3</span></span>|<span data-ttu-id="33d14-123">Legt fest, dass der eingebettete SIM Aktivierungscode auf das Zielgerät erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="33d14-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="33d14-124">Löschen</span><span class="sxs-lookup"><span data-stu-id="33d14-124">deleting</span></span>|<span data-ttu-id="33d14-125">4</span><span class="sxs-lookup"><span data-stu-id="33d14-125">4</span></span>|<span data-ttu-id="33d14-126">Legt fest, dass Intune Service versucht, um das Profil vom Gerät zu löschen.</span><span class="sxs-lookup"><span data-stu-id="33d14-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="33d14-127">error</span><span class="sxs-lookup"><span data-stu-id="33d14-127">error</span></span>|<span data-ttu-id="33d14-128">5</span><span class="sxs-lookup"><span data-stu-id="33d14-128">5</span></span>|<span data-ttu-id="33d14-129">Legt fest, dass Fehler mit diesem Profil vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="33d14-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="33d14-130">gelöscht</span><span class="sxs-lookup"><span data-stu-id="33d14-130">deleted</span></span>|<span data-ttu-id="33d14-131">6</span><span class="sxs-lookup"><span data-stu-id="33d14-131">6</span></span>|<span data-ttu-id="33d14-132">Legt fest, dass das Profil vom Gerät gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="33d14-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="33d14-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="33d14-133">removedByUser</span></span>|<span data-ttu-id="33d14-134">7</span><span class="sxs-lookup"><span data-stu-id="33d14-134">7</span></span>|<span data-ttu-id="33d14-135">Legt fest, dass das Profil des Benutzers vom Gerät entfernt wird</span><span class="sxs-lookup"><span data-stu-id="33d14-135">Designates that the profile is removed from the device by the user</span></span>|





