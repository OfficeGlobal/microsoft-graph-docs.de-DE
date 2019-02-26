---
title: appListType-Enumerationstyp
description: Mögliche Werte der Kompatibilitäts-App-Liste.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b7d11107ca3ea2b698e28cd288f163ec190b0a6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172674"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="b546f-103">appListType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="b546f-103">appListType enum type</span></span>

> <span data-ttu-id="b546f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b546f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b546f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b546f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b546f-106">Mögliche Werte der Kompatibilitäts-App-Liste.</span><span class="sxs-lookup"><span data-stu-id="b546f-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="b546f-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="b546f-107">Members</span></span>
|<span data-ttu-id="b546f-108">Element</span><span class="sxs-lookup"><span data-stu-id="b546f-108">Member</span></span>|<span data-ttu-id="b546f-109">Wert</span><span class="sxs-lookup"><span data-stu-id="b546f-109">Value</span></span>|<span data-ttu-id="b546f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b546f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b546f-111">Keine</span><span class="sxs-lookup"><span data-stu-id="b546f-111">none</span></span>|<span data-ttu-id="b546f-112">0</span><span class="sxs-lookup"><span data-stu-id="b546f-112">0</span></span>|<span data-ttu-id="b546f-113">Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="b546f-113">Default value, no intent.</span></span>|
|<span data-ttu-id="b546f-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b546f-114">appsInListCompliant</span></span>|<span data-ttu-id="b546f-115">1</span><span class="sxs-lookup"><span data-stu-id="b546f-115">1</span></span>|<span data-ttu-id="b546f-116">Die Liste stellt die apps dar, die als kompatibel betrachtet werden (nur apps in der Liste sind kompatibel).</span><span class="sxs-lookup"><span data-stu-id="b546f-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="b546f-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b546f-117">appsNotInListCompliant</span></span>|<span data-ttu-id="b546f-118">2</span><span class="sxs-lookup"><span data-stu-id="b546f-118">2</span></span>|<span data-ttu-id="b546f-119">Die Liste stellt die apps dar, die als nicht kompatibel gelten (alle apps sind mit Ausnahme von apps in der Liste kompatibel).</span><span class="sxs-lookup"><span data-stu-id="b546f-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




