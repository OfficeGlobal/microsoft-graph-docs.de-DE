---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425743"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="10c98-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="10c98-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="10c98-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="10c98-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="10c98-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10c98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10c98-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10c98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10c98-107">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="10c98-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="10c98-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="10c98-108">Members</span></span>
|<span data-ttu-id="10c98-109">Member</span><span class="sxs-lookup"><span data-stu-id="10c98-109">Member</span></span>|<span data-ttu-id="10c98-110">Wert</span><span class="sxs-lookup"><span data-stu-id="10c98-110">Value</span></span>|<span data-ttu-id="10c98-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10c98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10c98-112">noAction</span><span class="sxs-lookup"><span data-stu-id="10c98-112">noAction</span></span>|<span data-ttu-id="10c98-113">0</span><span class="sxs-lookup"><span data-stu-id="10c98-113">0</span></span>|<span data-ttu-id="10c98-114">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="10c98-114">No Action</span></span>|
|<span data-ttu-id="10c98-115">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="10c98-115">notification</span></span>|<span data-ttu-id="10c98-116">1</span><span class="sxs-lookup"><span data-stu-id="10c98-116">1</span></span>|<span data-ttu-id="10c98-117">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="10c98-117">Send Notification</span></span>|
|<span data-ttu-id="10c98-118">Blockieren</span><span class="sxs-lookup"><span data-stu-id="10c98-118">block</span></span>|<span data-ttu-id="10c98-119">2</span><span class="sxs-lookup"><span data-stu-id="10c98-119">2</span></span>|<span data-ttu-id="10c98-120">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="10c98-120">Block the device in AAD</span></span>|
|<span data-ttu-id="10c98-121">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="10c98-121">retire</span></span>|<span data-ttu-id="10c98-122">3</span><span class="sxs-lookup"><span data-stu-id="10c98-122">3</span></span>|<span data-ttu-id="10c98-123">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="10c98-123">Retire the device</span></span>|
|<span data-ttu-id="10c98-124">Wischen</span><span class="sxs-lookup"><span data-stu-id="10c98-124">wipe</span></span>|<span data-ttu-id="10c98-125">4</span><span class="sxs-lookup"><span data-stu-id="10c98-125">4</span></span>|<span data-ttu-id="10c98-126">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="10c98-126">Wipe the device</span></span>|
|<span data-ttu-id="10c98-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="10c98-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="10c98-128">5</span><span class="sxs-lookup"><span data-stu-id="10c98-128">5</span></span>|<span data-ttu-id="10c98-129">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="10c98-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="10c98-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="10c98-130">pushNotification</span></span>|<span data-ttu-id="10c98-131">9</span><span class="sxs-lookup"><span data-stu-id="10c98-131">9</span></span>|<span data-ttu-id="10c98-132">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="10c98-132">Send push notification to device</span></span>|
|<span data-ttu-id="10c98-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="10c98-133">remoteLock</span></span>|<span data-ttu-id="10c98-134">10</span><span class="sxs-lookup"><span data-stu-id="10c98-134">10</span></span>|<span data-ttu-id="10c98-135">Das Gerät Remote Sperren</span><span class="sxs-lookup"><span data-stu-id="10c98-135">Remotely lock the device</span></span>|




