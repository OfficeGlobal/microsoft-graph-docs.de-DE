---
title: appListType-Enumerationstyp
description: Mögliche Werte der Kompatibilitäts-App-Liste.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254324"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="02eae-103">appListType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="02eae-103">appListType enum type</span></span>

> <span data-ttu-id="02eae-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="02eae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02eae-105">Mögliche Werte der Kompatibilitäts-App-Liste.</span><span class="sxs-lookup"><span data-stu-id="02eae-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="02eae-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="02eae-106">Members</span></span>
|<span data-ttu-id="02eae-107">Element</span><span class="sxs-lookup"><span data-stu-id="02eae-107">Member</span></span>|<span data-ttu-id="02eae-108">Wert</span><span class="sxs-lookup"><span data-stu-id="02eae-108">Value</span></span>|<span data-ttu-id="02eae-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02eae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02eae-110">Keine</span><span class="sxs-lookup"><span data-stu-id="02eae-110">none</span></span>|<span data-ttu-id="02eae-111">0</span><span class="sxs-lookup"><span data-stu-id="02eae-111">0</span></span>|<span data-ttu-id="02eae-112">Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="02eae-112">Default value, no intent.</span></span>|
|<span data-ttu-id="02eae-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="02eae-113">appsInListCompliant</span></span>|<span data-ttu-id="02eae-114">1</span><span class="sxs-lookup"><span data-stu-id="02eae-114">1</span></span>|<span data-ttu-id="02eae-115">Die Liste stellt die apps dar, die als kompatibel betrachtet werden (nur apps in der Liste sind kompatibel).</span><span class="sxs-lookup"><span data-stu-id="02eae-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="02eae-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="02eae-116">appsNotInListCompliant</span></span>|<span data-ttu-id="02eae-117">2</span><span class="sxs-lookup"><span data-stu-id="02eae-117">2</span></span>|<span data-ttu-id="02eae-118">Die Liste stellt die apps dar, die als nicht kompatibel gelten (alle apps sind mit Ausnahme von apps in der Liste kompatibel).</span><span class="sxs-lookup"><span data-stu-id="02eae-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



