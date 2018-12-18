---
title: AppListType Enum-Typ
description: Mögliche Werte der Liste app Compliance.
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354719"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="98dee-103">AppListType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="98dee-103">appListType enum type</span></span>

> <span data-ttu-id="98dee-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="98dee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98dee-105">Mögliche Werte der Liste app Compliance.</span><span class="sxs-lookup"><span data-stu-id="98dee-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="98dee-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="98dee-106">Members</span></span>
|<span data-ttu-id="98dee-107">Member</span><span class="sxs-lookup"><span data-stu-id="98dee-107">Member</span></span>|<span data-ttu-id="98dee-108">Wert</span><span class="sxs-lookup"><span data-stu-id="98dee-108">Value</span></span>|<span data-ttu-id="98dee-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98dee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98dee-110">Keine</span><span class="sxs-lookup"><span data-stu-id="98dee-110">none</span></span>|<span data-ttu-id="98dee-111">0</span><span class="sxs-lookup"><span data-stu-id="98dee-111">0</span></span>|<span data-ttu-id="98dee-112">Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="98dee-112">Default value, no intent.</span></span>|
|<span data-ttu-id="98dee-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="98dee-113">appsInListCompliant</span></span>|<span data-ttu-id="98dee-114">1</span><span class="sxs-lookup"><span data-stu-id="98dee-114">1</span></span>|<span data-ttu-id="98dee-115">Die Liste darstellt, die apps, die kompatible berücksichtigt werden (nur in der Liste apps kompatibel sind).</span><span class="sxs-lookup"><span data-stu-id="98dee-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="98dee-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="98dee-116">appsNotInListCompliant</span></span>|<span data-ttu-id="98dee-117">2</span><span class="sxs-lookup"><span data-stu-id="98dee-117">2</span></span>|<span data-ttu-id="98dee-118">Die Liste darstellt, die apps, die nicht kompatible berücksichtigt werden (alle apps sind kompatibel mit Ausnahme von apps in der Liste).</span><span class="sxs-lookup"><span data-stu-id="98dee-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



