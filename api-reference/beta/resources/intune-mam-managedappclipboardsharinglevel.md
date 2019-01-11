---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
localization_priority: Normal
ms.openlocfilehash: 363e80b2242f5ac4d481389633aaa72fcc27894a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808176"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="e14b7-103">ManagedAppClipboardSharingLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e14b7-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="e14b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e14b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e14b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e14b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e14b7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e14b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e14b7-107">Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e14b7-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="e14b7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e14b7-108">Members</span></span>
|<span data-ttu-id="e14b7-109">Element</span><span class="sxs-lookup"><span data-stu-id="e14b7-109">Member</span></span>|<span data-ttu-id="e14b7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e14b7-110">Value</span></span>|<span data-ttu-id="e14b7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e14b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e14b7-112">allApps</span><span class="sxs-lookup"><span data-stu-id="e14b7-112">allApps</span></span>|<span data-ttu-id="e14b7-113">0</span><span class="sxs-lookup"><span data-stu-id="e14b7-113">0</span></span>|<span data-ttu-id="e14b7-114">Freigabe zwischen alle apps, verwaltete oder nicht zulässig</span><span class="sxs-lookup"><span data-stu-id="e14b7-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="e14b7-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="e14b7-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="e14b7-116">1</span><span class="sxs-lookup"><span data-stu-id="e14b7-116">1</span></span>|<span data-ttu-id="e14b7-117">Freigabe ist zulässig zwischen alle verwalteten apps mit Einfügen in aktiviert</span><span class="sxs-lookup"><span data-stu-id="e14b7-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="e14b7-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="e14b7-118">managedApps</span></span>|<span data-ttu-id="e14b7-119">2</span><span class="sxs-lookup"><span data-stu-id="e14b7-119">2</span></span>|<span data-ttu-id="e14b7-120">Freigabe ist zwischen alle verwalteten apps zulässig.</span><span class="sxs-lookup"><span data-stu-id="e14b7-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="e14b7-121">gesperrt</span><span class="sxs-lookup"><span data-stu-id="e14b7-121">blocked</span></span>|<span data-ttu-id="e14b7-122">3</span><span class="sxs-lookup"><span data-stu-id="e14b7-122">3</span></span>|<span data-ttu-id="e14b7-123">Freigabe von zwischen apps ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="e14b7-123">Sharing between apps is disabled</span></span>|





