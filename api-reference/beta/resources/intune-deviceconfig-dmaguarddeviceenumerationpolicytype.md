---
title: dmaGuardDeviceEnumerationPolicyType-Enumerationstyp
description: Mögliche Werte des DmaGuardDeviceEnumerationPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 512bf44d25629f4b1c88c2309c464e9d0f33f625
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159710"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="81afa-103">dmaGuardDeviceEnumerationPolicyType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="81afa-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="81afa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81afa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81afa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="81afa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81afa-106">Mögliche Werte des DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="81afa-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="81afa-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="81afa-107">Members</span></span>
|<span data-ttu-id="81afa-108">Element</span><span class="sxs-lookup"><span data-stu-id="81afa-108">Member</span></span>|<span data-ttu-id="81afa-109">Wert</span><span class="sxs-lookup"><span data-stu-id="81afa-109">Value</span></span>|<span data-ttu-id="81afa-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81afa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81afa-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="81afa-111">deviceDefault</span></span>|<span data-ttu-id="81afa-112">0</span><span class="sxs-lookup"><span data-stu-id="81afa-112">0</span></span>|<span data-ttu-id="81afa-113">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="81afa-113">Default value.</span></span> <span data-ttu-id="81afa-114">Geräte mit inkompatiblen DMA-Treibern werden nur aufgelistet, nachdem der Benutzer den Bildschirm aufgehoben hat.</span><span class="sxs-lookup"><span data-stu-id="81afa-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="81afa-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="81afa-115">blockAll</span></span>|<span data-ttu-id="81afa-116">1</span><span class="sxs-lookup"><span data-stu-id="81afa-116">1</span></span>|<span data-ttu-id="81afa-117">Geräte mit inkompatiblen DMA-Treibern können nie mehr gestartet und DMA ausführen.</span><span class="sxs-lookup"><span data-stu-id="81afa-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="81afa-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="81afa-118">allowAll</span></span>|<span data-ttu-id="81afa-119">2</span><span class="sxs-lookup"><span data-stu-id="81afa-119">2</span></span>|<span data-ttu-id="81afa-120">Alle externen DMA-fähigen PCIe-Geräte werden jederzeit aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="81afa-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




