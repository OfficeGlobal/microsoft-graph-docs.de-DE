---
title: WindowsSModeConfiguration Enum-Typ
description: Entsperren die möglichen Optionen S-Modus konfigurieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 858be5b3a55fbbf4454aa576785ba793f501079c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415467"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="7436a-103">WindowsSModeConfiguration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7436a-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="7436a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7436a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7436a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7436a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7436a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7436a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7436a-107">Entsperren die möglichen Optionen S-Modus konfigurieren</span><span class="sxs-lookup"><span data-stu-id="7436a-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="7436a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="7436a-108">Members</span></span>
|<span data-ttu-id="7436a-109">Member</span><span class="sxs-lookup"><span data-stu-id="7436a-109">Member</span></span>|<span data-ttu-id="7436a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7436a-110">Value</span></span>|<span data-ttu-id="7436a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7436a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7436a-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="7436a-112">noRestriction</span></span>|<span data-ttu-id="7436a-113">0</span><span class="sxs-lookup"><span data-stu-id="7436a-113">0</span></span>|<span data-ttu-id="7436a-114">Diese Option entfernt alle Einschränkungen zum Entsperren S Modus - Standard</span><span class="sxs-lookup"><span data-stu-id="7436a-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="7436a-115">Blockieren</span><span class="sxs-lookup"><span data-stu-id="7436a-115">block</span></span>|<span data-ttu-id="7436a-116">1</span><span class="sxs-lookup"><span data-stu-id="7436a-116">1</span></span>|<span data-ttu-id="7436a-117">Diese Option wird den Benutzer zum Entsperren des Geräts vom S Modus blockiert.</span><span class="sxs-lookup"><span data-stu-id="7436a-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="7436a-118">Entsperren</span><span class="sxs-lookup"><span data-stu-id="7436a-118">unlock</span></span>|<span data-ttu-id="7436a-119">2</span><span class="sxs-lookup"><span data-stu-id="7436a-119">2</span></span>|<span data-ttu-id="7436a-120">Diese Option wird das Gerät vom S Modus entsperren.</span><span class="sxs-lookup"><span data-stu-id="7436a-120">This option will unlock the device from S mode</span></span>|




