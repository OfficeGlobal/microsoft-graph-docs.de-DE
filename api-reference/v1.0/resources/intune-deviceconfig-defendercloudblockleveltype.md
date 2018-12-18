---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
author: tfitzmac
ms.openlocfilehash: 19c101cc82673009a39d6545f7340fabf65b287a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326614"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="0c392-103">DefenderCloudBlockLevelType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0c392-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="0c392-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0c392-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c392-105">Mögliche Werte für die Cloud Blockebene</span><span class="sxs-lookup"><span data-stu-id="0c392-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="0c392-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="0c392-106">Members</span></span>
|<span data-ttu-id="0c392-107">Member</span><span class="sxs-lookup"><span data-stu-id="0c392-107">Member</span></span>|<span data-ttu-id="0c392-108">Wert</span><span class="sxs-lookup"><span data-stu-id="0c392-108">Value</span></span>|<span data-ttu-id="0c392-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c392-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c392-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="0c392-110">notConfigured</span></span>|<span data-ttu-id="0c392-111">0</span><span class="sxs-lookup"><span data-stu-id="0c392-111">0</span></span>|<span data-ttu-id="0c392-112">Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien</span><span class="sxs-lookup"><span data-stu-id="0c392-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="0c392-113">hohe</span><span class="sxs-lookup"><span data-stu-id="0c392-113">high</span></span>|<span data-ttu-id="0c392-114">1</span><span class="sxs-lookup"><span data-stu-id="0c392-114">1</span></span>|<span data-ttu-id="0c392-115">Besonders weist eine starke Sicherheitsstufe Erkennung.</span><span class="sxs-lookup"><span data-stu-id="0c392-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="0c392-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="0c392-116">highPlus</span></span>|<span data-ttu-id="0c392-117">2</span><span class="sxs-lookup"><span data-stu-id="0c392-117">2</span></span>|<span data-ttu-id="0c392-118">Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition</span><span class="sxs-lookup"><span data-stu-id="0c392-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="0c392-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="0c392-119">zeroTolerance</span></span>|<span data-ttu-id="0c392-120">3</span><span class="sxs-lookup"><span data-stu-id="0c392-120">3</span></span>|<span data-ttu-id="0c392-121">0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="0c392-121">Zero tolerance blocks all unknown executables</span></span>|



