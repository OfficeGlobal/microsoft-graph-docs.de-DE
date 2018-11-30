---
title: DeviceThreatProtectionLevel Enum-Typ
description: Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
ms.openlocfilehash: 9b6a5066c26dcfe5ee2922bc736cf0292b1d3055
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019487"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="bd48a-103">DeviceThreatProtectionLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="bd48a-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="bd48a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd48a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd48a-105">Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.</span><span class="sxs-lookup"><span data-stu-id="bd48a-105">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="bd48a-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="bd48a-106">Members</span></span>
|<span data-ttu-id="bd48a-107">Element</span><span class="sxs-lookup"><span data-stu-id="bd48a-107">Member</span></span>|<span data-ttu-id="bd48a-108">Wert</span><span class="sxs-lookup"><span data-stu-id="bd48a-108">Value</span></span>|<span data-ttu-id="bd48a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd48a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd48a-110">nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="bd48a-110">unavailable</span></span>|<span data-ttu-id="bd48a-111">0</span><span class="sxs-lookup"><span data-stu-id="bd48a-111">0</span></span>|<span data-ttu-id="bd48a-112">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="bd48a-112">Default Value.</span></span> <span data-ttu-id="bd48a-113">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="bd48a-113">Do not use.</span></span>|
|<span data-ttu-id="bd48a-114">gesichert</span><span class="sxs-lookup"><span data-stu-id="bd48a-114">secured</span></span>|<span data-ttu-id="bd48a-115">1</span><span class="sxs-lookup"><span data-stu-id="bd48a-115">1</span></span>|<span data-ttu-id="bd48a-116">Gerät veränderte Anforderung: gesichert.</span><span class="sxs-lookup"><span data-stu-id="bd48a-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="bd48a-117">Dies ist die sicherste Ebene und steht, die auf dem Gerät keine Viren gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="bd48a-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="bd48a-118">Niedrig</span><span class="sxs-lookup"><span data-stu-id="bd48a-118">low</span></span>|<span data-ttu-id="bd48a-119">2</span><span class="sxs-lookup"><span data-stu-id="bd48a-119">2</span></span>|<span data-ttu-id="bd48a-120">Gerät Threat Protection geforderte: niedrig.</span><span class="sxs-lookup"><span data-stu-id="bd48a-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="bd48a-121">Niedrig stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten minimalem Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="bd48a-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="bd48a-122">medium</span><span class="sxs-lookup"><span data-stu-id="bd48a-122">medium</span></span>|<span data-ttu-id="bd48a-123">3</span><span class="sxs-lookup"><span data-stu-id="bd48a-123">3</span></span>|<span data-ttu-id="bd48a-124">Gerät Threat Protection geforderte: Mittel.</span><span class="sxs-lookup"><span data-stu-id="bd48a-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="bd48a-125">Mittel stellt einen Schweregrad der Bedrohung, dass Posen Risiko an das Gerät oder Gerätedaten mäßig dar.</span><span class="sxs-lookup"><span data-stu-id="bd48a-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="bd48a-126">hohe</span><span class="sxs-lookup"><span data-stu-id="bd48a-126">high</span></span>|<span data-ttu-id="bd48a-127">4</span><span class="sxs-lookup"><span data-stu-id="bd48a-127">4</span></span>|<span data-ttu-id="bd48a-128">Gerät Threat Protection geforderte: hoch.</span><span class="sxs-lookup"><span data-stu-id="bd48a-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="bd48a-129">Besonders stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten erheblich Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="bd48a-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="bd48a-130">notSet</span><span class="sxs-lookup"><span data-stu-id="bd48a-130">notSet</span></span>|<span data-ttu-id="bd48a-131">10</span><span class="sxs-lookup"><span data-stu-id="bd48a-131">10</span></span>|<span data-ttu-id="bd48a-132">Gerät Threat Protection geforderte: nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="bd48a-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="bd48a-133">Set darstellt, keine Notwendigkeit für das Gerät besteht zu eine Bedrohung Schutzebene erfüllen.</span><span class="sxs-lookup"><span data-stu-id="bd48a-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|


