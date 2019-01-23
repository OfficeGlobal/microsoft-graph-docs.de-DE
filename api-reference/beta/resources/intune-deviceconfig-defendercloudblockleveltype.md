---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425911"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="25af6-103">DefenderCloudBlockLevelType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="25af6-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="25af6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="25af6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25af6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25af6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25af6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25af6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25af6-107">Mögliche Werte für die Cloud Blockebene</span><span class="sxs-lookup"><span data-stu-id="25af6-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="25af6-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="25af6-108">Members</span></span>
|<span data-ttu-id="25af6-109">Member</span><span class="sxs-lookup"><span data-stu-id="25af6-109">Member</span></span>|<span data-ttu-id="25af6-110">Wert</span><span class="sxs-lookup"><span data-stu-id="25af6-110">Value</span></span>|<span data-ttu-id="25af6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25af6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25af6-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="25af6-112">notConfigured</span></span>|<span data-ttu-id="25af6-113">0</span><span class="sxs-lookup"><span data-stu-id="25af6-113">0</span></span>|<span data-ttu-id="25af6-114">Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien</span><span class="sxs-lookup"><span data-stu-id="25af6-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="25af6-115">hohe</span><span class="sxs-lookup"><span data-stu-id="25af6-115">high</span></span>|<span data-ttu-id="25af6-116">1</span><span class="sxs-lookup"><span data-stu-id="25af6-116">1</span></span>|<span data-ttu-id="25af6-117">Besonders weist eine starke Sicherheitsstufe Erkennung.</span><span class="sxs-lookup"><span data-stu-id="25af6-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="25af6-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="25af6-118">highPlus</span></span>|<span data-ttu-id="25af6-119">2</span><span class="sxs-lookup"><span data-stu-id="25af6-119">2</span></span>|<span data-ttu-id="25af6-120">Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition</span><span class="sxs-lookup"><span data-stu-id="25af6-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="25af6-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="25af6-121">zeroTolerance</span></span>|<span data-ttu-id="25af6-122">3</span><span class="sxs-lookup"><span data-stu-id="25af6-122">3</span></span>|<span data-ttu-id="25af6-123">0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="25af6-123">Zero tolerance blocks all unknown executables</span></span>|




