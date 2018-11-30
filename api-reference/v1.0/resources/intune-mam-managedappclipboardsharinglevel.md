---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
ms.openlocfilehash: 7cf7b4a2f6ea6dc129a21167a2d75ba215ff29fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020039"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="17f25-103">ManagedAppClipboardSharingLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="17f25-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="17f25-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="17f25-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17f25-105">Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird</span><span class="sxs-lookup"><span data-stu-id="17f25-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="17f25-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="17f25-106">Members</span></span>
|<span data-ttu-id="17f25-107">Element</span><span class="sxs-lookup"><span data-stu-id="17f25-107">Member</span></span>|<span data-ttu-id="17f25-108">Wert</span><span class="sxs-lookup"><span data-stu-id="17f25-108">Value</span></span>|<span data-ttu-id="17f25-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17f25-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f25-110">allApps</span><span class="sxs-lookup"><span data-stu-id="17f25-110">allApps</span></span>|<span data-ttu-id="17f25-111">0</span><span class="sxs-lookup"><span data-stu-id="17f25-111">0</span></span>|<span data-ttu-id="17f25-112">Freigabe zwischen alle apps, verwaltete oder nicht zulässig</span><span class="sxs-lookup"><span data-stu-id="17f25-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="17f25-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="17f25-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="17f25-114">1</span><span class="sxs-lookup"><span data-stu-id="17f25-114">1</span></span>|<span data-ttu-id="17f25-115">Freigabe ist zulässig zwischen alle verwalteten apps mit Einfügen in aktiviert</span><span class="sxs-lookup"><span data-stu-id="17f25-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="17f25-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="17f25-116">managedApps</span></span>|<span data-ttu-id="17f25-117">2</span><span class="sxs-lookup"><span data-stu-id="17f25-117">2</span></span>|<span data-ttu-id="17f25-118">Freigabe ist zwischen alle verwalteten apps zulässig.</span><span class="sxs-lookup"><span data-stu-id="17f25-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="17f25-119">gesperrt</span><span class="sxs-lookup"><span data-stu-id="17f25-119">blocked</span></span>|<span data-ttu-id="17f25-120">3</span><span class="sxs-lookup"><span data-stu-id="17f25-120">3</span></span>|<span data-ttu-id="17f25-121">Freigabe von zwischen apps ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="17f25-121">Sharing between apps is disabled</span></span>|



