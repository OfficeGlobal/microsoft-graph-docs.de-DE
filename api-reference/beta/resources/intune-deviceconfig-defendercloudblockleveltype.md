---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
author: tfitzmac
ms.openlocfilehash: c58c844097c18ff86beaef4a0e48d9b8a39043f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317444"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="e8c7f-103">DefenderCloudBlockLevelType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e8c7f-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="e8c7f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8c7f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8c7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8c7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8c7f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e8c7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8c7f-107">Mögliche Werte für die Cloud Blockebene</span><span class="sxs-lookup"><span data-stu-id="e8c7f-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="e8c7f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e8c7f-108">Members</span></span>
|<span data-ttu-id="e8c7f-109">Member</span><span class="sxs-lookup"><span data-stu-id="e8c7f-109">Member</span></span>|<span data-ttu-id="e8c7f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e8c7f-110">Value</span></span>|<span data-ttu-id="e8c7f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8c7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8c7f-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="e8c7f-112">notConfigured</span></span>|<span data-ttu-id="e8c7f-113">0</span><span class="sxs-lookup"><span data-stu-id="e8c7f-113">0</span></span>|<span data-ttu-id="e8c7f-114">Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien</span><span class="sxs-lookup"><span data-stu-id="e8c7f-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="e8c7f-115">hohe</span><span class="sxs-lookup"><span data-stu-id="e8c7f-115">high</span></span>|<span data-ttu-id="e8c7f-116">1</span><span class="sxs-lookup"><span data-stu-id="e8c7f-116">1</span></span>|<span data-ttu-id="e8c7f-117">Besonders weist eine starke Sicherheitsstufe Erkennung.</span><span class="sxs-lookup"><span data-stu-id="e8c7f-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="e8c7f-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="e8c7f-118">highPlus</span></span>|<span data-ttu-id="e8c7f-119">2</span><span class="sxs-lookup"><span data-stu-id="e8c7f-119">2</span></span>|<span data-ttu-id="e8c7f-120">Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition</span><span class="sxs-lookup"><span data-stu-id="e8c7f-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="e8c7f-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="e8c7f-121">zeroTolerance</span></span>|<span data-ttu-id="e8c7f-122">3</span><span class="sxs-lookup"><span data-stu-id="e8c7f-122">3</span></span>|<span data-ttu-id="e8c7f-123">0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="e8c7f-123">Zero tolerance blocks all unknown executables</span></span>|





