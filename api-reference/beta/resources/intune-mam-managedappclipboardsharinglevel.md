---
title: managedAppClipboardSharingLevel-Enumerationstyp
description: Stellt die Ebene dar, in der die Zwischenablage des Geräts zwischen apps freigegeben werden kann.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 352a801c53acd487fdac0206eca828461d35bf68
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148349"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="b29e1-103">managedAppClipboardSharingLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="b29e1-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="b29e1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b29e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b29e1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b29e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b29e1-106">Stellt die Ebene dar, in der die Zwischenablage des Geräts zwischen apps freigegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="b29e1-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="b29e1-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="b29e1-107">Members</span></span>
|<span data-ttu-id="b29e1-108">Element</span><span class="sxs-lookup"><span data-stu-id="b29e1-108">Member</span></span>|<span data-ttu-id="b29e1-109">Wert</span><span class="sxs-lookup"><span data-stu-id="b29e1-109">Value</span></span>|<span data-ttu-id="b29e1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b29e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b29e1-111">allApps</span><span class="sxs-lookup"><span data-stu-id="b29e1-111">allApps</span></span>|<span data-ttu-id="b29e1-112">0</span><span class="sxs-lookup"><span data-stu-id="b29e1-112">0</span></span>|<span data-ttu-id="b29e1-113">Freigabe ist zwischen allen apps zulässig, verwaltet oder nicht</span><span class="sxs-lookup"><span data-stu-id="b29e1-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="b29e1-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="b29e1-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="b29e1-115">1</span><span class="sxs-lookup"><span data-stu-id="b29e1-115">1</span></span>|<span data-ttu-id="b29e1-116">Freigabe ist zwischen allen verwalteten apps zulässig, wobei Paste aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b29e1-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="b29e1-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="b29e1-117">managedApps</span></span>|<span data-ttu-id="b29e1-118">2</span><span class="sxs-lookup"><span data-stu-id="b29e1-118">2</span></span>|<span data-ttu-id="b29e1-119">Freigabe ist zwischen allen verwalteten apps zulässig</span><span class="sxs-lookup"><span data-stu-id="b29e1-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="b29e1-120">gesperrt</span><span class="sxs-lookup"><span data-stu-id="b29e1-120">blocked</span></span>|<span data-ttu-id="b29e1-121">3</span><span class="sxs-lookup"><span data-stu-id="b29e1-121">3</span></span>|<span data-ttu-id="b29e1-122">Die Freigabe zwischen Apps ist deaktiviert</span><span class="sxs-lookup"><span data-stu-id="b29e1-122">Sharing between apps is disabled</span></span>|




