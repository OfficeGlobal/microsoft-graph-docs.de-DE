---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 13f8828478eb063eaa25d8561d5a254c86f4b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924720"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="233df-103">DefenderCloudBlockLevelType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="233df-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="233df-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="233df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="233df-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="233df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="233df-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="233df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="233df-107">Mögliche Werte für die Cloud Blockebene</span><span class="sxs-lookup"><span data-stu-id="233df-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="233df-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="233df-108">Members</span></span>
|<span data-ttu-id="233df-109">Element</span><span class="sxs-lookup"><span data-stu-id="233df-109">Member</span></span>|<span data-ttu-id="233df-110">Wert</span><span class="sxs-lookup"><span data-stu-id="233df-110">Value</span></span>|<span data-ttu-id="233df-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="233df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="233df-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="233df-112">notConfigured</span></span>|<span data-ttu-id="233df-113">0</span><span class="sxs-lookup"><span data-stu-id="233df-113">0</span></span>|<span data-ttu-id="233df-114">Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien</span><span class="sxs-lookup"><span data-stu-id="233df-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="233df-115">hohe</span><span class="sxs-lookup"><span data-stu-id="233df-115">high</span></span>|<span data-ttu-id="233df-116">1</span><span class="sxs-lookup"><span data-stu-id="233df-116">1</span></span>|<span data-ttu-id="233df-117">Besonders weist eine starke Sicherheitsstufe Erkennung.</span><span class="sxs-lookup"><span data-stu-id="233df-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="233df-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="233df-118">highPlus</span></span>|<span data-ttu-id="233df-119">2</span><span class="sxs-lookup"><span data-stu-id="233df-119">2</span></span>|<span data-ttu-id="233df-120">Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition</span><span class="sxs-lookup"><span data-stu-id="233df-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="233df-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="233df-121">zeroTolerance</span></span>|<span data-ttu-id="233df-122">3</span><span class="sxs-lookup"><span data-stu-id="233df-122">3</span></span>|<span data-ttu-id="233df-123">0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="233df-123">Zero tolerance blocks all unknown executables</span></span>|





