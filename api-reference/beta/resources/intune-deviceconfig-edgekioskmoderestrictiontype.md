---
title: edgeKioskModeRestrictionType-Enumerationstyp
description: Geben Sie an, wie die Microsoft-Edgeeinstellungen basierend auf dem Kioskmodus eingeschränkt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0dcd1d30895acbdecf9d9cc706ee14b7907f14f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177959"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="991a4-103">edgeKioskModeRestrictionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="991a4-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="991a4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="991a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="991a4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="991a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="991a4-106">Geben Sie an, wie die Microsoft-Edgeeinstellungen basierend auf dem Kioskmodus eingeschränkt werden.</span><span class="sxs-lookup"><span data-stu-id="991a4-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="991a4-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="991a4-107">Members</span></span>
|<span data-ttu-id="991a4-108">Element</span><span class="sxs-lookup"><span data-stu-id="991a4-108">Member</span></span>|<span data-ttu-id="991a4-109">Wert</span><span class="sxs-lookup"><span data-stu-id="991a4-109">Value</span></span>|<span data-ttu-id="991a4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="991a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="991a4-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="991a4-111">notConfigured</span></span>|<span data-ttu-id="991a4-112">0</span><span class="sxs-lookup"><span data-stu-id="991a4-112">0</span></span>|<span data-ttu-id="991a4-113">Nicht konfiguriert (Unrestricted).</span><span class="sxs-lookup"><span data-stu-id="991a4-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="991a4-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="991a4-114">digitalSignage</span></span>|<span data-ttu-id="991a4-115">1</span><span class="sxs-lookup"><span data-stu-id="991a4-115">1</span></span>|<span data-ttu-id="991a4-116">Interaktive/digitale Beschilderung im Einzel-APP-Modus.</span><span class="sxs-lookup"><span data-stu-id="991a4-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="991a4-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="991a4-117">normalMode</span></span>|<span data-ttu-id="991a4-118">2</span><span class="sxs-lookup"><span data-stu-id="991a4-118">2</span></span>|<span data-ttu-id="991a4-119">Normaler Modus (Vollversion von Microsoft Edge).</span><span class="sxs-lookup"><span data-stu-id="991a4-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="991a4-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="991a4-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="991a4-121">3</span><span class="sxs-lookup"><span data-stu-id="991a4-121">3</span></span>|<span data-ttu-id="991a4-122">Öffentliches Browsen im Einzel-APP-Modus.</span><span class="sxs-lookup"><span data-stu-id="991a4-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="991a4-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="991a4-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="991a4-124">4</span><span class="sxs-lookup"><span data-stu-id="991a4-124">4</span></span>|<span data-ttu-id="991a4-125">Öffentliches Browsen (inPrivate) im Multi-APP-Modus.</span><span class="sxs-lookup"><span data-stu-id="991a4-125">Public browsing (inPrivate) in multi-app mode.</span></span>|




