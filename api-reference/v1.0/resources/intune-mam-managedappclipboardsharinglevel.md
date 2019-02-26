---
title: managedAppClipboardSharingLevel-Enumerationstyp
description: Stellt die Ebene dar, in der die Zwischenablage des Geräts zwischen apps freigegeben werden kann.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250026"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="4b738-103">managedAppClipboardSharingLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="4b738-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="4b738-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4b738-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b738-105">Stellt die Ebene dar, in der die Zwischenablage des Geräts zwischen apps freigegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="4b738-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="4b738-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="4b738-106">Members</span></span>
|<span data-ttu-id="4b738-107">Element</span><span class="sxs-lookup"><span data-stu-id="4b738-107">Member</span></span>|<span data-ttu-id="4b738-108">Wert</span><span class="sxs-lookup"><span data-stu-id="4b738-108">Value</span></span>|<span data-ttu-id="4b738-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b738-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b738-110">allApps</span><span class="sxs-lookup"><span data-stu-id="4b738-110">allApps</span></span>|<span data-ttu-id="4b738-111">0</span><span class="sxs-lookup"><span data-stu-id="4b738-111">0</span></span>|<span data-ttu-id="4b738-112">Freigabe ist zwischen allen apps zulässig, verwaltet oder nicht</span><span class="sxs-lookup"><span data-stu-id="4b738-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="4b738-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="4b738-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="4b738-114">1</span><span class="sxs-lookup"><span data-stu-id="4b738-114">1</span></span>|<span data-ttu-id="4b738-115">Freigabe ist zwischen allen verwalteten apps zulässig, wobei Paste aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4b738-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="4b738-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="4b738-116">managedApps</span></span>|<span data-ttu-id="4b738-117">2</span><span class="sxs-lookup"><span data-stu-id="4b738-117">2</span></span>|<span data-ttu-id="4b738-118">Freigabe ist zwischen allen verwalteten apps zulässig</span><span class="sxs-lookup"><span data-stu-id="4b738-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="4b738-119">gesperrt</span><span class="sxs-lookup"><span data-stu-id="4b738-119">blocked</span></span>|<span data-ttu-id="4b738-120">3</span><span class="sxs-lookup"><span data-stu-id="4b738-120">3</span></span>|<span data-ttu-id="4b738-121">Die Freigabe zwischen Apps ist deaktiviert</span><span class="sxs-lookup"><span data-stu-id="4b738-121">Sharing between apps is disabled</span></span>|



