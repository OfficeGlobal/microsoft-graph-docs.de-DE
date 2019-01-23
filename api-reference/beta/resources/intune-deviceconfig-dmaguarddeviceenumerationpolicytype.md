---
title: DmaGuardDeviceEnumerationPolicyType Enum-Typ
description: Mögliche Werte für die DmaGuardDeviceEnumerationPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430130"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="2ac1c-103">DmaGuardDeviceEnumerationPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="2ac1c-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="2ac1c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ac1c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ac1c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac1c-107">Mögliche Werte für die DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="2ac1c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="2ac1c-108">Members</span></span>
|<span data-ttu-id="2ac1c-109">Member</span><span class="sxs-lookup"><span data-stu-id="2ac1c-109">Member</span></span>|<span data-ttu-id="2ac1c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="2ac1c-110">Value</span></span>|<span data-ttu-id="2ac1c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ac1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac1c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2ac1c-112">deviceDefault</span></span>|<span data-ttu-id="2ac1c-113">0</span><span class="sxs-lookup"><span data-stu-id="2ac1c-113">0</span></span>|<span data-ttu-id="2ac1c-114">Standardwert.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-114">Default value.</span></span> <span data-ttu-id="2ac1c-115">Nachdem der Benutzer auf den Bildschirm entsperrt, werden nur Geräte mit DMA Neuzuordnen Treiber kompatibel aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="2ac1c-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="2ac1c-116">blockAll</span></span>|<span data-ttu-id="2ac1c-117">1</span><span class="sxs-lookup"><span data-stu-id="2ac1c-117">1</span></span>|<span data-ttu-id="2ac1c-118">Geräte mit DMA Neuzuordnen inkompatiblen Treiber die nie zum Starten und Ausführen von DMA jederzeit zulässig.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="2ac1c-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="2ac1c-119">allowAll</span></span>|<span data-ttu-id="2ac1c-120">2</span><span class="sxs-lookup"><span data-stu-id="2ac1c-120">2</span></span>|<span data-ttu-id="2ac1c-121">Alle externe DMA PCIe Geräten werden zu einem beliebigen Zeitpunkt aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="2ac1c-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




