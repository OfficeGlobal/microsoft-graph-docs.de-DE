---
title: managedAppFlaggedReason-Enumerationstyp
description: Der Grund für die Kennzeichnung eines Benutzers
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15942be9f9b6d8b25941f0726ff6046feeea386b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572159"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="ecb70-103">managedAppFlaggedReason-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="ecb70-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="ecb70-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ecb70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecb70-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ecb70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecb70-106">Der Grund für die Kennzeichnung eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="ecb70-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="ecb70-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="ecb70-107">Members</span></span>
|<span data-ttu-id="ecb70-108">Element</span><span class="sxs-lookup"><span data-stu-id="ecb70-108">Member</span></span>|<span data-ttu-id="ecb70-109">Wert</span><span class="sxs-lookup"><span data-stu-id="ecb70-109">Value</span></span>|<span data-ttu-id="ecb70-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecb70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecb70-111">Keine</span><span class="sxs-lookup"><span data-stu-id="ecb70-111">none</span></span>|<span data-ttu-id="ecb70-112">0</span><span class="sxs-lookup"><span data-stu-id="ecb70-112">0</span></span>|<span data-ttu-id="ecb70-113">Kein Problem.</span><span class="sxs-lookup"><span data-stu-id="ecb70-113">No issue.</span></span>|
|<span data-ttu-id="ecb70-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="ecb70-114">rootedDevice</span></span>|<span data-ttu-id="ecb70-115">1</span><span class="sxs-lookup"><span data-stu-id="ecb70-115">1</span></span>|<span data-ttu-id="ecb70-116">Die APP-Registrierung läuft auf einem Rooted/Unlocked-Gerät.</span><span class="sxs-lookup"><span data-stu-id="ecb70-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="ecb70-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="ecb70-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="ecb70-118">2</span><span class="sxs-lookup"><span data-stu-id="ecb70-118">2</span></span>|<span data-ttu-id="ecb70-119">Die APP-Registrierung wird auf einem Android-Gerät gestartet, auf dem der Bootloader entriegelt ist.</span><span class="sxs-lookup"><span data-stu-id="ecb70-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="ecb70-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="ecb70-120">androidFactoryRomModified</span></span>|<span data-ttu-id="ecb70-121">3</span><span class="sxs-lookup"><span data-stu-id="ecb70-121">3</span></span>|<span data-ttu-id="ecb70-122">Die APP-Registrierung wird auf einem Android-Gerät ausgeführt, auf dem die Factory-ROM geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="ecb70-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|




