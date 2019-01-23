---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410987"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="59283-103">ManagedAppClipboardSharingLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="59283-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="59283-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="59283-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59283-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59283-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59283-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59283-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59283-107">Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird</span><span class="sxs-lookup"><span data-stu-id="59283-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="59283-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="59283-108">Members</span></span>
|<span data-ttu-id="59283-109">Member</span><span class="sxs-lookup"><span data-stu-id="59283-109">Member</span></span>|<span data-ttu-id="59283-110">Wert</span><span class="sxs-lookup"><span data-stu-id="59283-110">Value</span></span>|<span data-ttu-id="59283-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59283-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59283-112">allApps</span><span class="sxs-lookup"><span data-stu-id="59283-112">allApps</span></span>|<span data-ttu-id="59283-113">0</span><span class="sxs-lookup"><span data-stu-id="59283-113">0</span></span>|<span data-ttu-id="59283-114">Freigabe zwischen alle apps, verwaltete oder nicht zulässig</span><span class="sxs-lookup"><span data-stu-id="59283-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="59283-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="59283-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="59283-116">1</span><span class="sxs-lookup"><span data-stu-id="59283-116">1</span></span>|<span data-ttu-id="59283-117">Freigabe ist zulässig zwischen alle verwalteten apps mit Einfügen in aktiviert</span><span class="sxs-lookup"><span data-stu-id="59283-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="59283-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="59283-118">managedApps</span></span>|<span data-ttu-id="59283-119">2</span><span class="sxs-lookup"><span data-stu-id="59283-119">2</span></span>|<span data-ttu-id="59283-120">Freigabe ist zwischen alle verwalteten apps zulässig.</span><span class="sxs-lookup"><span data-stu-id="59283-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="59283-121">gesperrt</span><span class="sxs-lookup"><span data-stu-id="59283-121">blocked</span></span>|<span data-ttu-id="59283-122">3</span><span class="sxs-lookup"><span data-stu-id="59283-122">3</span></span>|<span data-ttu-id="59283-123">Freigabe von zwischen apps ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="59283-123">Sharing between apps is disabled</span></span>|




