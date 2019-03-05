---
title: defenderCloudBlockLevelType-Enumerationstyp
description: Mögliche Werte der Cloud-Blockebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258835"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="8f46a-103">defenderCloudBlockLevelType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="8f46a-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="8f46a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8f46a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f46a-105">Mögliche Werte der Cloud-Blockebene</span><span class="sxs-lookup"><span data-stu-id="8f46a-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="8f46a-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="8f46a-106">Members</span></span>
|<span data-ttu-id="8f46a-107">Element</span><span class="sxs-lookup"><span data-stu-id="8f46a-107">Member</span></span>|<span data-ttu-id="8f46a-108">Wert</span><span class="sxs-lookup"><span data-stu-id="8f46a-108">Value</span></span>|<span data-ttu-id="8f46a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f46a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f46a-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8f46a-110">notConfigured</span></span>|<span data-ttu-id="8f46a-111">0</span><span class="sxs-lookup"><span data-stu-id="8f46a-111">0</span></span>|<span data-ttu-id="8f46a-112">Standardwert, verwendet die standardmäßige Windows Defender-Antivirus-Blockierungs Ebene und bietet eine starke Erkennung, ohne das Risiko der Erkennung legitimer Dateien zu erhöhen</span><span class="sxs-lookup"><span data-stu-id="8f46a-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="8f46a-113">hohe</span><span class="sxs-lookup"><span data-stu-id="8f46a-113">high</span></span>|<span data-ttu-id="8f46a-114">1</span><span class="sxs-lookup"><span data-stu-id="8f46a-114">1</span></span>|<span data-ttu-id="8f46a-115">High gilt als starke Erkennungsstufe.</span><span class="sxs-lookup"><span data-stu-id="8f46a-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="8f46a-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="8f46a-116">highPlus</span></span>|<span data-ttu-id="8f46a-117">2</span><span class="sxs-lookup"><span data-stu-id="8f46a-117">2</span></span>|<span data-ttu-id="8f46a-118">High + verwendet den hohen Level und wendet zusätzliche Schutzmaßnahmen an.</span><span class="sxs-lookup"><span data-stu-id="8f46a-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="8f46a-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="8f46a-119">zeroTolerance</span></span>|<span data-ttu-id="8f46a-120">3</span><span class="sxs-lookup"><span data-stu-id="8f46a-120">3</span></span>|<span data-ttu-id="8f46a-121">Null Toleranz blockiert alle unbekannten ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="8f46a-121">Zero tolerance blocks all unknown executables</span></span>|



