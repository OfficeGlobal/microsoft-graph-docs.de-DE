---
title: deviceThreatProtectionLevel-Enumerationstyp
description: Geräte Bedrohungsschutz-Ebenen für die Geräte BedrohungsSchutz-API.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ecdf54051b1545b842cbc3c49359b9a77f12e2e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140243"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="1dce3-103">deviceThreatProtectionLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="1dce3-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="1dce3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1dce3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dce3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1dce3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dce3-106">Geräte Bedrohungsschutz-Ebenen für die Geräte BedrohungsSchutz-API.</span><span class="sxs-lookup"><span data-stu-id="1dce3-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="1dce3-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1dce3-107">Members</span></span>
|<span data-ttu-id="1dce3-108">Element</span><span class="sxs-lookup"><span data-stu-id="1dce3-108">Member</span></span>|<span data-ttu-id="1dce3-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1dce3-109">Value</span></span>|<span data-ttu-id="1dce3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dce3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dce3-111">verfügbar</span><span class="sxs-lookup"><span data-stu-id="1dce3-111">unavailable</span></span>|<span data-ttu-id="1dce3-112">0</span><span class="sxs-lookup"><span data-stu-id="1dce3-112">0</span></span>|<span data-ttu-id="1dce3-113">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="1dce3-113">Default Value.</span></span> <span data-ttu-id="1dce3-114">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="1dce3-114">Do not use.</span></span>|
|<span data-ttu-id="1dce3-115">gesichert</span><span class="sxs-lookup"><span data-stu-id="1dce3-115">secured</span></span>|<span data-ttu-id="1dce3-116">1</span><span class="sxs-lookup"><span data-stu-id="1dce3-116">1</span></span>|<span data-ttu-id="1dce3-117">Anforderung der Geräte BedrohungsStufe: gesichert.</span><span class="sxs-lookup"><span data-stu-id="1dce3-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="1dce3-118">Dies ist die sicherste Stufe und stellt dar, dass auf dem Gerät keine Bedrohungen gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="1dce3-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="1dce3-119">mit niedriger</span><span class="sxs-lookup"><span data-stu-id="1dce3-119">low</span></span>|<span data-ttu-id="1dce3-120">2</span><span class="sxs-lookup"><span data-stu-id="1dce3-120">2</span></span>|<span data-ttu-id="1dce3-121">Anforderung an die Geräte Bedrohungsstufe: niedrig.</span><span class="sxs-lookup"><span data-stu-id="1dce3-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="1dce3-122">Low stellt einen Schweregrad der Bedrohung dar, der ein minimales Risiko für die Geräte-oder Gerätedaten darstellt.</span><span class="sxs-lookup"><span data-stu-id="1dce3-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="1dce3-123">medium</span><span class="sxs-lookup"><span data-stu-id="1dce3-123">medium</span></span>|<span data-ttu-id="1dce3-124">3</span><span class="sxs-lookup"><span data-stu-id="1dce3-124">3</span></span>|<span data-ttu-id="1dce3-125">Anforderung der Geräte BedrohungsSchutz Stufe: Mittel.</span><span class="sxs-lookup"><span data-stu-id="1dce3-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="1dce3-126">Medium stellt einen Schweregrad der Bedrohung dar, der für die Geräte-oder Gerätedaten ein moderates Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="1dce3-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="1dce3-127">hohe</span><span class="sxs-lookup"><span data-stu-id="1dce3-127">high</span></span>|<span data-ttu-id="1dce3-128">4</span><span class="sxs-lookup"><span data-stu-id="1dce3-128">4</span></span>|<span data-ttu-id="1dce3-129">Anforderung an Geräte BedrohungsSchutz: hoch.</span><span class="sxs-lookup"><span data-stu-id="1dce3-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="1dce3-130">High stellt einen Schweregrad der Bedrohung dar, der für die Geräte-oder Gerätedaten ein hohes Risiko birgt.</span><span class="sxs-lookup"><span data-stu-id="1dce3-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="1dce3-131">notSet</span><span class="sxs-lookup"><span data-stu-id="1dce3-131">notSet</span></span>|<span data-ttu-id="1dce3-132">10</span><span class="sxs-lookup"><span data-stu-id="1dce3-132">10</span></span>|<span data-ttu-id="1dce3-133">Anforderung der Geräte BedrohungsSchutz Ebene: nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1dce3-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="1dce3-134">Nicht festgelegt stellt dar, dass das Gerät keine BedrohungsSchutz Ebene erfüllen muss.</span><span class="sxs-lookup"><span data-stu-id="1dce3-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




