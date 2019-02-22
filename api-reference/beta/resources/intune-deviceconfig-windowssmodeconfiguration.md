---
title: windowsSModeConfiguration-Enumerationstyp
description: Die möglichen Optionen zum Konfigurieren des S-Modus entsperren
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a451108c6e55f8587317dfc43caf8bc84cca673
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144716"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="83968-103">windowsSModeConfiguration-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="83968-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="83968-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83968-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83968-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="83968-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83968-106">Die möglichen Optionen zum Konfigurieren des S-Modus entsperren</span><span class="sxs-lookup"><span data-stu-id="83968-106">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="83968-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="83968-107">Members</span></span>
|<span data-ttu-id="83968-108">Element</span><span class="sxs-lookup"><span data-stu-id="83968-108">Member</span></span>|<span data-ttu-id="83968-109">Wert</span><span class="sxs-lookup"><span data-stu-id="83968-109">Value</span></span>|<span data-ttu-id="83968-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83968-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83968-111">noRestriction</span><span class="sxs-lookup"><span data-stu-id="83968-111">noRestriction</span></span>|<span data-ttu-id="83968-112">0</span><span class="sxs-lookup"><span data-stu-id="83968-112">0</span></span>|<span data-ttu-id="83968-113">Mit dieser Option werden alle Einschränkungen für den Unlock-Modus-Standard</span><span class="sxs-lookup"><span data-stu-id="83968-113">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="83968-114">Block</span><span class="sxs-lookup"><span data-stu-id="83968-114">block</span></span>|<span data-ttu-id="83968-115">1</span><span class="sxs-lookup"><span data-stu-id="83968-115">1</span></span>|<span data-ttu-id="83968-116">Mit dieser Option wird verhindert, dass der Benutzer das Gerät im S-Modus entsperren kann.</span><span class="sxs-lookup"><span data-stu-id="83968-116">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="83968-117">Entsperren</span><span class="sxs-lookup"><span data-stu-id="83968-117">unlock</span></span>|<span data-ttu-id="83968-118">2</span><span class="sxs-lookup"><span data-stu-id="83968-118">2</span></span>|<span data-ttu-id="83968-119">Mit dieser Option wird das Gerät im S-Modus gesperrt.</span><span class="sxs-lookup"><span data-stu-id="83968-119">This option will unlock the device from S mode</span></span>|




