---
title: defenderCloudBlockLevelType-Enumerationstyp
description: Mögliche Werte der Cloud-Blockebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbf442a11335602c510a210d7bd805b2a76eb7df
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156924"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="1af7c-103">defenderCloudBlockLevelType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="1af7c-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="1af7c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1af7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1af7c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1af7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af7c-106">Mögliche Werte der Cloud-Blockebene</span><span class="sxs-lookup"><span data-stu-id="1af7c-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="1af7c-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1af7c-107">Members</span></span>
|<span data-ttu-id="1af7c-108">Element</span><span class="sxs-lookup"><span data-stu-id="1af7c-108">Member</span></span>|<span data-ttu-id="1af7c-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1af7c-109">Value</span></span>|<span data-ttu-id="1af7c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1af7c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af7c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1af7c-111">notConfigured</span></span>|<span data-ttu-id="1af7c-112">0</span><span class="sxs-lookup"><span data-stu-id="1af7c-112">0</span></span>|<span data-ttu-id="1af7c-113">Standardwert, verwendet die standardmäßige Windows Defender-Antivirus-Blockierungs Ebene und bietet eine starke Erkennung, ohne das Risiko der Erkennung legitimer Dateien zu erhöhen</span><span class="sxs-lookup"><span data-stu-id="1af7c-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="1af7c-114">hohe</span><span class="sxs-lookup"><span data-stu-id="1af7c-114">high</span></span>|<span data-ttu-id="1af7c-115">1</span><span class="sxs-lookup"><span data-stu-id="1af7c-115">1</span></span>|<span data-ttu-id="1af7c-116">High gilt als starke Erkennungsstufe.</span><span class="sxs-lookup"><span data-stu-id="1af7c-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="1af7c-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="1af7c-117">highPlus</span></span>|<span data-ttu-id="1af7c-118">2</span><span class="sxs-lookup"><span data-stu-id="1af7c-118">2</span></span>|<span data-ttu-id="1af7c-119">High + verwendet den hohen Level und wendet zusätzliche Schutzmaßnahmen an.</span><span class="sxs-lookup"><span data-stu-id="1af7c-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="1af7c-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="1af7c-120">zeroTolerance</span></span>|<span data-ttu-id="1af7c-121">3</span><span class="sxs-lookup"><span data-stu-id="1af7c-121">3</span></span>|<span data-ttu-id="1af7c-122">Null Toleranz blockiert alle unbekannten ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="1af7c-122">Zero tolerance blocks all unknown executables</span></span>|




