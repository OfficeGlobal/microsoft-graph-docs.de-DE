---
title: deviceComplianceActionType-Enumerationstyp
description: Enum für geplante Aktionstypen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd370f9e706955d76de519a518b4659ba46c6d25
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250915"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="fdd69-103">deviceComplianceActionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="fdd69-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="fdd69-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fdd69-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdd69-105">Enum für geplante Aktionstypen</span><span class="sxs-lookup"><span data-stu-id="fdd69-105">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="fdd69-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="fdd69-106">Members</span></span>
|<span data-ttu-id="fdd69-107">Element</span><span class="sxs-lookup"><span data-stu-id="fdd69-107">Member</span></span>|<span data-ttu-id="fdd69-108">Wert</span><span class="sxs-lookup"><span data-stu-id="fdd69-108">Value</span></span>|<span data-ttu-id="fdd69-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdd69-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdd69-110">noAction</span><span class="sxs-lookup"><span data-stu-id="fdd69-110">noAction</span></span>|<span data-ttu-id="fdd69-111">0</span><span class="sxs-lookup"><span data-stu-id="fdd69-111">0</span></span>|<span data-ttu-id="fdd69-112">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="fdd69-112">No Action</span></span>|
|<span data-ttu-id="fdd69-113">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="fdd69-113">notification</span></span>|<span data-ttu-id="fdd69-114">1</span><span class="sxs-lookup"><span data-stu-id="fdd69-114">1</span></span>|<span data-ttu-id="fdd69-115">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="fdd69-115">Send Notification</span></span>|
|<span data-ttu-id="fdd69-116">Block</span><span class="sxs-lookup"><span data-stu-id="fdd69-116">block</span></span>|<span data-ttu-id="fdd69-117">2</span><span class="sxs-lookup"><span data-stu-id="fdd69-117">2</span></span>|<span data-ttu-id="fdd69-118">Blockieren des Geräts in AAD</span><span class="sxs-lookup"><span data-stu-id="fdd69-118">Block the device in AAD</span></span>|
|<span data-ttu-id="fdd69-119">zurückziehen</span><span class="sxs-lookup"><span data-stu-id="fdd69-119">retire</span></span>|<span data-ttu-id="fdd69-120">3</span><span class="sxs-lookup"><span data-stu-id="fdd69-120">3</span></span>|<span data-ttu-id="fdd69-121">Zurückziehen des Geräts</span><span class="sxs-lookup"><span data-stu-id="fdd69-121">Retire the device</span></span>|
|<span data-ttu-id="fdd69-122">Zurücksetzung</span><span class="sxs-lookup"><span data-stu-id="fdd69-122">wipe</span></span>|<span data-ttu-id="fdd69-123">4</span><span class="sxs-lookup"><span data-stu-id="fdd69-123">4</span></span>|<span data-ttu-id="fdd69-124">Wischen Sie das Gerät ab.</span><span class="sxs-lookup"><span data-stu-id="fdd69-124">Wipe the device</span></span>|
|<span data-ttu-id="fdd69-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="fdd69-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="fdd69-126">5</span><span class="sxs-lookup"><span data-stu-id="fdd69-126">5</span></span>|<span data-ttu-id="fdd69-127">Entfernen von Ressourcenzugriffs Profilen vom Gerät</span><span class="sxs-lookup"><span data-stu-id="fdd69-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="fdd69-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="fdd69-128">pushNotification</span></span>|<span data-ttu-id="fdd69-129">9</span><span class="sxs-lookup"><span data-stu-id="fdd69-129">9</span></span>|<span data-ttu-id="fdd69-130">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="fdd69-130">Send push notification to device</span></span>|



