---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 283bb12c775b1215a1bcfecf4f248882a56573aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839501"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="a131a-103">DefenderCloudBlockLevelType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a131a-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="a131a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a131a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a131a-105">Mögliche Werte für die Cloud Blockebene</span><span class="sxs-lookup"><span data-stu-id="a131a-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="a131a-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="a131a-106">Members</span></span>
|<span data-ttu-id="a131a-107">Element</span><span class="sxs-lookup"><span data-stu-id="a131a-107">Member</span></span>|<span data-ttu-id="a131a-108">Wert</span><span class="sxs-lookup"><span data-stu-id="a131a-108">Value</span></span>|<span data-ttu-id="a131a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a131a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a131a-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="a131a-110">notConfigured</span></span>|<span data-ttu-id="a131a-111">0</span><span class="sxs-lookup"><span data-stu-id="a131a-111">0</span></span>|<span data-ttu-id="a131a-112">Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien</span><span class="sxs-lookup"><span data-stu-id="a131a-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="a131a-113">hohe</span><span class="sxs-lookup"><span data-stu-id="a131a-113">high</span></span>|<span data-ttu-id="a131a-114">1</span><span class="sxs-lookup"><span data-stu-id="a131a-114">1</span></span>|<span data-ttu-id="a131a-115">Besonders weist eine starke Sicherheitsstufe Erkennung.</span><span class="sxs-lookup"><span data-stu-id="a131a-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="a131a-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="a131a-116">highPlus</span></span>|<span data-ttu-id="a131a-117">2</span><span class="sxs-lookup"><span data-stu-id="a131a-117">2</span></span>|<span data-ttu-id="a131a-118">Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition</span><span class="sxs-lookup"><span data-stu-id="a131a-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="a131a-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="a131a-119">zeroTolerance</span></span>|<span data-ttu-id="a131a-120">3</span><span class="sxs-lookup"><span data-stu-id="a131a-120">3</span></span>|<span data-ttu-id="a131a-121">0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="a131a-121">Zero tolerance blocks all unknown executables</span></span>|



