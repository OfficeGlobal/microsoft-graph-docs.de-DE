---
title: WindowsSModeConfiguration Enum-Typ
description: Entsperren die möglichen Optionen S-Modus konfigurieren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28106a073a6bb213fe17e80193cb32d1e6b3b9ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947379"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="18f41-103">WindowsSModeConfiguration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="18f41-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="18f41-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18f41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18f41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18f41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18f41-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="18f41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18f41-107">Entsperren die möglichen Optionen S-Modus konfigurieren</span><span class="sxs-lookup"><span data-stu-id="18f41-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="18f41-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="18f41-108">Members</span></span>
|<span data-ttu-id="18f41-109">Element</span><span class="sxs-lookup"><span data-stu-id="18f41-109">Member</span></span>|<span data-ttu-id="18f41-110">Wert</span><span class="sxs-lookup"><span data-stu-id="18f41-110">Value</span></span>|<span data-ttu-id="18f41-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18f41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f41-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="18f41-112">noRestriction</span></span>|<span data-ttu-id="18f41-113">0</span><span class="sxs-lookup"><span data-stu-id="18f41-113">0</span></span>|<span data-ttu-id="18f41-114">Diese Option entfernt alle Einschränkungen zum Entsperren S Modus - Standard</span><span class="sxs-lookup"><span data-stu-id="18f41-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="18f41-115">Blockieren</span><span class="sxs-lookup"><span data-stu-id="18f41-115">block</span></span>|<span data-ttu-id="18f41-116">1</span><span class="sxs-lookup"><span data-stu-id="18f41-116">1</span></span>|<span data-ttu-id="18f41-117">Diese Option wird den Benutzer zum Entsperren des Geräts vom S Modus blockiert.</span><span class="sxs-lookup"><span data-stu-id="18f41-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="18f41-118">Entsperren</span><span class="sxs-lookup"><span data-stu-id="18f41-118">unlock</span></span>|<span data-ttu-id="18f41-119">2</span><span class="sxs-lookup"><span data-stu-id="18f41-119">2</span></span>|<span data-ttu-id="18f41-120">Diese Option wird das Gerät vom S Modus entsperren.</span><span class="sxs-lookup"><span data-stu-id="18f41-120">This option will unlock the device from S mode</span></span>|





