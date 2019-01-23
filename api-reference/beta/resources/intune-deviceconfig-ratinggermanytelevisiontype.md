---
title: RatingGermanyTelevisionType Enum-Typ
description: TV zum Bewerten Bezeichnungen in Deutschland
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9bbe383b13e5a6f3d9ec704977b284eaf740aed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424616"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="33b95-103">RatingGermanyTelevisionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="33b95-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="33b95-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="33b95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33b95-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33b95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33b95-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33b95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b95-107">TV zum Bewerten Bezeichnungen in Deutschland</span><span class="sxs-lookup"><span data-stu-id="33b95-107">TV content rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="33b95-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="33b95-108">Members</span></span>
|<span data-ttu-id="33b95-109">Member</span><span class="sxs-lookup"><span data-stu-id="33b95-109">Member</span></span>|<span data-ttu-id="33b95-110">Wert</span><span class="sxs-lookup"><span data-stu-id="33b95-110">Value</span></span>|<span data-ttu-id="33b95-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33b95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b95-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="33b95-112">allAllowed</span></span>|<span data-ttu-id="33b95-113">0</span><span class="sxs-lookup"><span data-stu-id="33b95-113">0</span></span>|<span data-ttu-id="33b95-114">Standardwert, zulassen, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="33b95-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="33b95-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="33b95-115">allBlocked</span></span>|<span data-ttu-id="33b95-116">1</span><span class="sxs-lookup"><span data-stu-id="33b95-116">1</span></span>|<span data-ttu-id="33b95-117">Lassen Sie nicht, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="33b95-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="33b95-118">Allgemeine</span><span class="sxs-lookup"><span data-stu-id="33b95-118">general</span></span>|<span data-ttu-id="33b95-119">2</span><span class="sxs-lookup"><span data-stu-id="33b95-119">2</span></span>|<span data-ttu-id="33b95-120">Ab 0 Jahren, ohne Einschränkungen ALTER</span><span class="sxs-lookup"><span data-stu-id="33b95-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="33b95-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="33b95-121">agesAbove6</span></span>|<span data-ttu-id="33b95-122">3</span><span class="sxs-lookup"><span data-stu-id="33b95-122">3</span></span>|<span data-ttu-id="33b95-123">Ab 6 Jahren, im Alter zwischen 6 und ältere</span><span class="sxs-lookup"><span data-stu-id="33b95-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="33b95-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="33b95-124">agesAbove12</span></span>|<span data-ttu-id="33b95-125">4</span><span class="sxs-lookup"><span data-stu-id="33b95-125">4</span></span>|<span data-ttu-id="33b95-126">Ab 12 Jahren, Alter 12 und ältere</span><span class="sxs-lookup"><span data-stu-id="33b95-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="33b95-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="33b95-127">agesAbove16</span></span>|<span data-ttu-id="33b95-128">5</span><span class="sxs-lookup"><span data-stu-id="33b95-128">5</span></span>|<span data-ttu-id="33b95-129">Ab 16 Jahren, im Alter zwischen 16 und ältere</span><span class="sxs-lookup"><span data-stu-id="33b95-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="33b95-130">Erwachsene</span><span class="sxs-lookup"><span data-stu-id="33b95-130">adults</span></span>|<span data-ttu-id="33b95-131">6</span><span class="sxs-lookup"><span data-stu-id="33b95-131">6</span></span>|<span data-ttu-id="33b95-132">Ab 18 Jahren, nur Erwachsene</span><span class="sxs-lookup"><span data-stu-id="33b95-132">Ab 18 Jahren, adults only</span></span>|




