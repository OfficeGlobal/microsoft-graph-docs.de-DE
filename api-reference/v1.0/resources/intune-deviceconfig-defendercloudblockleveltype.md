---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
ms.openlocfilehash: 6ea336418a90a3d4caeab074cb71fce997ea1275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018024"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="dffee-103">DefenderCloudBlockLevelType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="dffee-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="dffee-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dffee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dffee-105">Mögliche Werte für die Cloud Blockebene</span><span class="sxs-lookup"><span data-stu-id="dffee-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="dffee-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="dffee-106">Members</span></span>
|<span data-ttu-id="dffee-107">Element</span><span class="sxs-lookup"><span data-stu-id="dffee-107">Member</span></span>|<span data-ttu-id="dffee-108">Wert</span><span class="sxs-lookup"><span data-stu-id="dffee-108">Value</span></span>|<span data-ttu-id="dffee-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dffee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dffee-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="dffee-110">notConfigured</span></span>|<span data-ttu-id="dffee-111">0</span><span class="sxs-lookup"><span data-stu-id="dffee-111">0</span></span>|<span data-ttu-id="dffee-112">Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien</span><span class="sxs-lookup"><span data-stu-id="dffee-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="dffee-113">hohe</span><span class="sxs-lookup"><span data-stu-id="dffee-113">high</span></span>|<span data-ttu-id="dffee-114">1</span><span class="sxs-lookup"><span data-stu-id="dffee-114">1</span></span>|<span data-ttu-id="dffee-115">Besonders weist eine starke Sicherheitsstufe Erkennung.</span><span class="sxs-lookup"><span data-stu-id="dffee-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="dffee-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="dffee-116">highPlus</span></span>|<span data-ttu-id="dffee-117">2</span><span class="sxs-lookup"><span data-stu-id="dffee-117">2</span></span>|<span data-ttu-id="dffee-118">Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition</span><span class="sxs-lookup"><span data-stu-id="dffee-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="dffee-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="dffee-119">zeroTolerance</span></span>|<span data-ttu-id="dffee-120">3</span><span class="sxs-lookup"><span data-stu-id="dffee-120">3</span></span>|<span data-ttu-id="dffee-121">0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="dffee-121">Zero tolerance blocks all unknown executables</span></span>|



