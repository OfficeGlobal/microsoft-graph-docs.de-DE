---
title: DeviceThreatProtectionLevel Enum-Typ
description: Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d4c17fc9883b23417a4c72ac7cc3c75512865c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948051"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="93db0-103">DeviceThreatProtectionLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="93db0-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="93db0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93db0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93db0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93db0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93db0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93db0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93db0-107">Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.</span><span class="sxs-lookup"><span data-stu-id="93db0-107">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="93db0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="93db0-108">Members</span></span>
|<span data-ttu-id="93db0-109">Element</span><span class="sxs-lookup"><span data-stu-id="93db0-109">Member</span></span>|<span data-ttu-id="93db0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="93db0-110">Value</span></span>|<span data-ttu-id="93db0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93db0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93db0-112">nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="93db0-112">unavailable</span></span>|<span data-ttu-id="93db0-113">0</span><span class="sxs-lookup"><span data-stu-id="93db0-113">0</span></span>|<span data-ttu-id="93db0-114">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="93db0-114">Default Value.</span></span> <span data-ttu-id="93db0-115">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="93db0-115">Do not use.</span></span>|
|<span data-ttu-id="93db0-116">gesichert</span><span class="sxs-lookup"><span data-stu-id="93db0-116">secured</span></span>|<span data-ttu-id="93db0-117">1</span><span class="sxs-lookup"><span data-stu-id="93db0-117">1</span></span>|<span data-ttu-id="93db0-118">Gerät veränderte Anforderung: gesichert.</span><span class="sxs-lookup"><span data-stu-id="93db0-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="93db0-119">Dies ist die sicherste Ebene und steht, die auf dem Gerät keine Viren gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="93db0-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="93db0-120">Niedrig</span><span class="sxs-lookup"><span data-stu-id="93db0-120">low</span></span>|<span data-ttu-id="93db0-121">2</span><span class="sxs-lookup"><span data-stu-id="93db0-121">2</span></span>|<span data-ttu-id="93db0-122">Gerät Threat Protection geforderte: niedrig.</span><span class="sxs-lookup"><span data-stu-id="93db0-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="93db0-123">Niedrig stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten minimalem Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="93db0-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="93db0-124">medium</span><span class="sxs-lookup"><span data-stu-id="93db0-124">medium</span></span>|<span data-ttu-id="93db0-125">3</span><span class="sxs-lookup"><span data-stu-id="93db0-125">3</span></span>|<span data-ttu-id="93db0-126">Gerät Threat Protection geforderte: Mittel.</span><span class="sxs-lookup"><span data-stu-id="93db0-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="93db0-127">Mittel stellt einen Schweregrad der Bedrohung, dass Posen Risiko an das Gerät oder Gerätedaten mäßig dar.</span><span class="sxs-lookup"><span data-stu-id="93db0-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="93db0-128">hohe</span><span class="sxs-lookup"><span data-stu-id="93db0-128">high</span></span>|<span data-ttu-id="93db0-129">4</span><span class="sxs-lookup"><span data-stu-id="93db0-129">4</span></span>|<span data-ttu-id="93db0-130">Gerät Threat Protection geforderte: hoch.</span><span class="sxs-lookup"><span data-stu-id="93db0-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="93db0-131">Besonders stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten erheblich Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="93db0-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="93db0-132">notSet</span><span class="sxs-lookup"><span data-stu-id="93db0-132">notSet</span></span>|<span data-ttu-id="93db0-133">10</span><span class="sxs-lookup"><span data-stu-id="93db0-133">10</span></span>|<span data-ttu-id="93db0-134">Gerät Threat Protection geforderte: nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="93db0-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="93db0-135">Set darstellt, keine Notwendigkeit für das Gerät besteht zu eine Bedrohung Schutzebene erfüllen.</span><span class="sxs-lookup"><span data-stu-id="93db0-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





