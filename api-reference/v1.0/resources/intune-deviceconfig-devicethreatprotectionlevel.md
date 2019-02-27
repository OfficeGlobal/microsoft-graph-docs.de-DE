---
title: deviceThreatProtectionLevel-Enumerationstyp
description: Geräte Bedrohungsschutz-Ebenen für die Geräte BedrohungsSchutz-API.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af0231e15cfa815d3fd2e154adf180f3e0c0c43
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253295"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="3179c-103">deviceThreatProtectionLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="3179c-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="3179c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3179c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3179c-105">Geräte Bedrohungsschutz-Ebenen für die Geräte BedrohungsSchutz-API.</span><span class="sxs-lookup"><span data-stu-id="3179c-105">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="3179c-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="3179c-106">Members</span></span>
|<span data-ttu-id="3179c-107">Element</span><span class="sxs-lookup"><span data-stu-id="3179c-107">Member</span></span>|<span data-ttu-id="3179c-108">Wert</span><span class="sxs-lookup"><span data-stu-id="3179c-108">Value</span></span>|<span data-ttu-id="3179c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3179c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3179c-110">verfügbar</span><span class="sxs-lookup"><span data-stu-id="3179c-110">unavailable</span></span>|<span data-ttu-id="3179c-111">0</span><span class="sxs-lookup"><span data-stu-id="3179c-111">0</span></span>|<span data-ttu-id="3179c-112">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="3179c-112">Default Value.</span></span> <span data-ttu-id="3179c-113">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="3179c-113">Do not use.</span></span>|
|<span data-ttu-id="3179c-114">gesichert</span><span class="sxs-lookup"><span data-stu-id="3179c-114">secured</span></span>|<span data-ttu-id="3179c-115">1</span><span class="sxs-lookup"><span data-stu-id="3179c-115">1</span></span>|<span data-ttu-id="3179c-116">Anforderung der Geräte BedrohungsStufe: gesichert.</span><span class="sxs-lookup"><span data-stu-id="3179c-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="3179c-117">Dies ist die sicherste Stufe und stellt dar, dass auf dem Gerät keine Bedrohungen gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="3179c-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="3179c-118">mit niedriger</span><span class="sxs-lookup"><span data-stu-id="3179c-118">low</span></span>|<span data-ttu-id="3179c-119">2</span><span class="sxs-lookup"><span data-stu-id="3179c-119">2</span></span>|<span data-ttu-id="3179c-120">Anforderung an die Geräte Bedrohungsstufe: niedrig.</span><span class="sxs-lookup"><span data-stu-id="3179c-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="3179c-121">Low stellt einen Schweregrad der Bedrohung dar, der ein minimales Risiko für die Geräte-oder Gerätedaten darstellt.</span><span class="sxs-lookup"><span data-stu-id="3179c-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="3179c-122">medium</span><span class="sxs-lookup"><span data-stu-id="3179c-122">medium</span></span>|<span data-ttu-id="3179c-123">3</span><span class="sxs-lookup"><span data-stu-id="3179c-123">3</span></span>|<span data-ttu-id="3179c-124">Anforderung der Geräte BedrohungsSchutz Stufe: Mittel.</span><span class="sxs-lookup"><span data-stu-id="3179c-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="3179c-125">Medium stellt einen Schweregrad der Bedrohung dar, der für die Geräte-oder Gerätedaten ein moderates Risiko darstellt.</span><span class="sxs-lookup"><span data-stu-id="3179c-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="3179c-126">hohe</span><span class="sxs-lookup"><span data-stu-id="3179c-126">high</span></span>|<span data-ttu-id="3179c-127">4</span><span class="sxs-lookup"><span data-stu-id="3179c-127">4</span></span>|<span data-ttu-id="3179c-128">Anforderung an Geräte BedrohungsSchutz: hoch.</span><span class="sxs-lookup"><span data-stu-id="3179c-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="3179c-129">High stellt einen Schweregrad der Bedrohung dar, der für die Geräte-oder Gerätedaten ein hohes Risiko birgt.</span><span class="sxs-lookup"><span data-stu-id="3179c-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="3179c-130">notSet</span><span class="sxs-lookup"><span data-stu-id="3179c-130">notSet</span></span>|<span data-ttu-id="3179c-131">10</span><span class="sxs-lookup"><span data-stu-id="3179c-131">10</span></span>|<span data-ttu-id="3179c-132">Anforderung der Geräte BedrohungsSchutz Ebene: nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3179c-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="3179c-133">Nicht festgelegt stellt dar, dass das Gerät keine BedrohungsSchutz Ebene erfüllen muss.</span><span class="sxs-lookup"><span data-stu-id="3179c-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



