---
title: DeviceThreatProtectionLevel Enum-Typ
description: Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411232"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="5e2a2-103">DeviceThreatProtectionLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5e2a2-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="5e2a2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e2a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e2a2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e2a2-107">Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="5e2a2-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5e2a2-108">Members</span></span>
|<span data-ttu-id="5e2a2-109">Member</span><span class="sxs-lookup"><span data-stu-id="5e2a2-109">Member</span></span>|<span data-ttu-id="5e2a2-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5e2a2-110">Value</span></span>|<span data-ttu-id="5e2a2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e2a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2a2-112">nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="5e2a2-112">unavailable</span></span>|<span data-ttu-id="5e2a2-113">0</span><span class="sxs-lookup"><span data-stu-id="5e2a2-113">0</span></span>|<span data-ttu-id="5e2a2-114">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-114">Default Value.</span></span> <span data-ttu-id="5e2a2-115">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-115">Do not use.</span></span>|
|<span data-ttu-id="5e2a2-116">gesichert</span><span class="sxs-lookup"><span data-stu-id="5e2a2-116">secured</span></span>|<span data-ttu-id="5e2a2-117">1</span><span class="sxs-lookup"><span data-stu-id="5e2a2-117">1</span></span>|<span data-ttu-id="5e2a2-118">Gerät veränderte Anforderung: gesichert.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="5e2a2-119">Dies ist die sicherste Ebene und steht, die auf dem Gerät keine Viren gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="5e2a2-120">Niedrig</span><span class="sxs-lookup"><span data-stu-id="5e2a2-120">low</span></span>|<span data-ttu-id="5e2a2-121">2</span><span class="sxs-lookup"><span data-stu-id="5e2a2-121">2</span></span>|<span data-ttu-id="5e2a2-122">Gerät Threat Protection geforderte: niedrig.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="5e2a2-123">Niedrig stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten minimalem Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="5e2a2-124">medium</span><span class="sxs-lookup"><span data-stu-id="5e2a2-124">medium</span></span>|<span data-ttu-id="5e2a2-125">3</span><span class="sxs-lookup"><span data-stu-id="5e2a2-125">3</span></span>|<span data-ttu-id="5e2a2-126">Gerät Threat Protection geforderte: Mittel.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="5e2a2-127">Mittel stellt einen Schweregrad der Bedrohung, dass Posen Risiko an das Gerät oder Gerätedaten mäßig dar.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="5e2a2-128">hohe</span><span class="sxs-lookup"><span data-stu-id="5e2a2-128">high</span></span>|<span data-ttu-id="5e2a2-129">4</span><span class="sxs-lookup"><span data-stu-id="5e2a2-129">4</span></span>|<span data-ttu-id="5e2a2-130">Gerät Threat Protection geforderte: hoch.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="5e2a2-131">Besonders stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten erheblich Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="5e2a2-132">notSet</span><span class="sxs-lookup"><span data-stu-id="5e2a2-132">notSet</span></span>|<span data-ttu-id="5e2a2-133">10</span><span class="sxs-lookup"><span data-stu-id="5e2a2-133">10</span></span>|<span data-ttu-id="5e2a2-134">Gerät Threat Protection geforderte: nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="5e2a2-135">Set darstellt, keine Notwendigkeit für das Gerät besteht zu eine Bedrohung Schutzebene erfüllen.</span><span class="sxs-lookup"><span data-stu-id="5e2a2-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




