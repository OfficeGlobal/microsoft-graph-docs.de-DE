---
title: AppListType Enum-Typ
description: Mögliche Werte der Liste app Compliance.
author: tfitzmac
ms.openlocfilehash: 3f0fa162131fc1f59beba1f057fa888e0f2260c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331192"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="53850-103">AppListType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="53850-103">appListType enum type</span></span>

> <span data-ttu-id="53850-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53850-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53850-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53850-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53850-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="53850-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53850-107">Mögliche Werte der Liste app Compliance.</span><span class="sxs-lookup"><span data-stu-id="53850-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="53850-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="53850-108">Members</span></span>
|<span data-ttu-id="53850-109">Member</span><span class="sxs-lookup"><span data-stu-id="53850-109">Member</span></span>|<span data-ttu-id="53850-110">Wert</span><span class="sxs-lookup"><span data-stu-id="53850-110">Value</span></span>|<span data-ttu-id="53850-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53850-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53850-112">Keine</span><span class="sxs-lookup"><span data-stu-id="53850-112">none</span></span>|<span data-ttu-id="53850-113">0</span><span class="sxs-lookup"><span data-stu-id="53850-113">0</span></span>|<span data-ttu-id="53850-114">Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="53850-114">Default value, no intent.</span></span>|
|<span data-ttu-id="53850-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="53850-115">appsInListCompliant</span></span>|<span data-ttu-id="53850-116">1</span><span class="sxs-lookup"><span data-stu-id="53850-116">1</span></span>|<span data-ttu-id="53850-117">Die Liste darstellt, die apps, die kompatible berücksichtigt werden (nur in der Liste apps kompatibel sind).</span><span class="sxs-lookup"><span data-stu-id="53850-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="53850-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="53850-118">appsNotInListCompliant</span></span>|<span data-ttu-id="53850-119">2</span><span class="sxs-lookup"><span data-stu-id="53850-119">2</span></span>|<span data-ttu-id="53850-120">Die Liste darstellt, die apps, die nicht kompatible berücksichtigt werden (alle apps sind kompatibel mit Ausnahme von apps in der Liste).</span><span class="sxs-lookup"><span data-stu-id="53850-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





