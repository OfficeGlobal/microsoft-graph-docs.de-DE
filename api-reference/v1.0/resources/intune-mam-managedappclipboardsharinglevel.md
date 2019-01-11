---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
localization_priority: Normal
ms.openlocfilehash: 16d6e9154b3d6e683d9ddce0efd70a40c01c8994
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814315"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="6a0d3-103">ManagedAppClipboardSharingLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6a0d3-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="6a0d3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6a0d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a0d3-105">Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6a0d3-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="6a0d3-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="6a0d3-106">Members</span></span>
|<span data-ttu-id="6a0d3-107">Element</span><span class="sxs-lookup"><span data-stu-id="6a0d3-107">Member</span></span>|<span data-ttu-id="6a0d3-108">Wert</span><span class="sxs-lookup"><span data-stu-id="6a0d3-108">Value</span></span>|<span data-ttu-id="6a0d3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a0d3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a0d3-110">allApps</span><span class="sxs-lookup"><span data-stu-id="6a0d3-110">allApps</span></span>|<span data-ttu-id="6a0d3-111">0</span><span class="sxs-lookup"><span data-stu-id="6a0d3-111">0</span></span>|<span data-ttu-id="6a0d3-112">Freigabe zwischen alle apps, verwaltete oder nicht zulässig</span><span class="sxs-lookup"><span data-stu-id="6a0d3-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="6a0d3-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="6a0d3-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="6a0d3-114">1</span><span class="sxs-lookup"><span data-stu-id="6a0d3-114">1</span></span>|<span data-ttu-id="6a0d3-115">Freigabe ist zulässig zwischen alle verwalteten apps mit Einfügen in aktiviert</span><span class="sxs-lookup"><span data-stu-id="6a0d3-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="6a0d3-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="6a0d3-116">managedApps</span></span>|<span data-ttu-id="6a0d3-117">2</span><span class="sxs-lookup"><span data-stu-id="6a0d3-117">2</span></span>|<span data-ttu-id="6a0d3-118">Freigabe ist zwischen alle verwalteten apps zulässig.</span><span class="sxs-lookup"><span data-stu-id="6a0d3-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="6a0d3-119">gesperrt</span><span class="sxs-lookup"><span data-stu-id="6a0d3-119">blocked</span></span>|<span data-ttu-id="6a0d3-120">3</span><span class="sxs-lookup"><span data-stu-id="6a0d3-120">3</span></span>|<span data-ttu-id="6a0d3-121">Freigabe von zwischen apps ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="6a0d3-121">Sharing between apps is disabled</span></span>|



