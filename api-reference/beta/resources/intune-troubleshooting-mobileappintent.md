---
title: MobileAppIntent Enum-Typ
description: Gibt den Status der mobilen app auf dem Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a807e89ec949c2c48f04af46b26f43b393cc4b0a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419261"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="6f94a-103">MobileAppIntent Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6f94a-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="6f94a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6f94a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f94a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f94a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f94a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f94a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f94a-107">Gibt den Status der mobilen app auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="6f94a-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="6f94a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="6f94a-108">Members</span></span>
|<span data-ttu-id="6f94a-109">Member</span><span class="sxs-lookup"><span data-stu-id="6f94a-109">Member</span></span>|<span data-ttu-id="6f94a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="6f94a-110">Value</span></span>|<span data-ttu-id="6f94a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f94a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f94a-112">Verfügbar</span><span class="sxs-lookup"><span data-stu-id="6f94a-112">available</span></span>|<span data-ttu-id="6f94a-113">0</span><span class="sxs-lookup"><span data-stu-id="6f94a-113">0</span></span>|<span data-ttu-id="6f94a-114">Available</span><span class="sxs-lookup"><span data-stu-id="6f94a-114">Available</span></span>|
|<span data-ttu-id="6f94a-115">nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="6f94a-115">notAvailable</span></span>|<span data-ttu-id="6f94a-116">1</span><span class="sxs-lookup"><span data-stu-id="6f94a-116">1</span></span>|<span data-ttu-id="6f94a-117">Nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="6f94a-117">Not Available</span></span>|
|<span data-ttu-id="6f94a-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="6f94a-118">requiredInstall</span></span>|<span data-ttu-id="6f94a-119">2</span><span class="sxs-lookup"><span data-stu-id="6f94a-119">2</span></span>|<span data-ttu-id="6f94a-120">Installation erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f94a-120">Required Install</span></span>|
|<span data-ttu-id="6f94a-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="6f94a-121">requiredUninstall</span></span>|<span data-ttu-id="6f94a-122">3</span><span class="sxs-lookup"><span data-stu-id="6f94a-122">3</span></span>|<span data-ttu-id="6f94a-123">Erforderliche Deinstallation</span><span class="sxs-lookup"><span data-stu-id="6f94a-123">Required Uninstall</span></span>|
|<span data-ttu-id="6f94a-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="6f94a-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="6f94a-125">4</span><span class="sxs-lookup"><span data-stu-id="6f94a-125">4</span></span>|<span data-ttu-id="6f94a-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="6f94a-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="6f94a-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="6f94a-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="6f94a-128">5</span><span class="sxs-lookup"><span data-stu-id="6f94a-128">5</span></span>|<span data-ttu-id="6f94a-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="6f94a-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="6f94a-130">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="6f94a-130">exclude</span></span>|<span data-ttu-id="6f94a-131">6</span><span class="sxs-lookup"><span data-stu-id="6f94a-131">6</span></span>|<span data-ttu-id="6f94a-132">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="6f94a-132">Exclude</span></span>|




