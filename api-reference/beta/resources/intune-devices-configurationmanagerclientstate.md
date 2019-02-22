---
title: configurationManagerClientState-Enumerationstyp
description: Konfigurations-Manager-Client – Status
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8474e6886c1312fde4ce3afde3c3fe0185574c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170700"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="d1d74-103">configurationManagerClientState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="d1d74-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="d1d74-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1d74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1d74-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d1d74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1d74-106">Konfigurations-Manager-Client – Status</span><span class="sxs-lookup"><span data-stu-id="d1d74-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="d1d74-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="d1d74-107">Members</span></span>
|<span data-ttu-id="d1d74-108">Element</span><span class="sxs-lookup"><span data-stu-id="d1d74-108">Member</span></span>|<span data-ttu-id="d1d74-109">Wert</span><span class="sxs-lookup"><span data-stu-id="d1d74-109">Value</span></span>|<span data-ttu-id="d1d74-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1d74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1d74-111">unknown</span><span class="sxs-lookup"><span data-stu-id="d1d74-111">unknown</span></span>|<span data-ttu-id="d1d74-112">0</span><span class="sxs-lookup"><span data-stu-id="d1d74-112">0</span></span>|<span data-ttu-id="d1d74-113">Der Configuration Manager-Agent ist älter als 1806 oder nicht installiert, oder dieses Gerät wurde seit über 30 Tagen nicht in InTune eingecheckt.</span><span class="sxs-lookup"><span data-stu-id="d1d74-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="d1d74-114">installiert</span><span class="sxs-lookup"><span data-stu-id="d1d74-114">installed</span></span>|<span data-ttu-id="d1d74-115">1</span><span class="sxs-lookup"><span data-stu-id="d1d74-115">1</span></span>|<span data-ttu-id="d1d74-116">Der Configuration Manager-Agent ist installiert, wird jedoch möglicherweise noch nicht in der Configuration Manager-Konsole angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d1d74-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="d1d74-117">Warten Sie einige Stunden, bis es aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="d1d74-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="d1d74-118">gesunde</span><span class="sxs-lookup"><span data-stu-id="d1d74-118">healthy</span></span>|<span data-ttu-id="d1d74-119">7</span><span class="sxs-lookup"><span data-stu-id="d1d74-119">7</span></span>|<span data-ttu-id="d1d74-120">Dieses Gerät konnte den Configuration Manager-Dienst erfolgreich einchecken.</span><span class="sxs-lookup"><span data-stu-id="d1d74-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="d1d74-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="d1d74-121">installFailed</span></span>|<span data-ttu-id="d1d74-122">8</span><span class="sxs-lookup"><span data-stu-id="d1d74-122">8</span></span>|<span data-ttu-id="d1d74-123">Fehler beim Installieren des Configuration Manager-Agents.</span><span class="sxs-lookup"><span data-stu-id="d1d74-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="d1d74-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="d1d74-124">updateFailed</span></span>|<span data-ttu-id="d1d74-125">11</span><span class="sxs-lookup"><span data-stu-id="d1d74-125">11</span></span>|<span data-ttu-id="d1d74-126">Fehler bei der Aktualisierung von Version x auf Version y des Configuration Manager-Agents.</span><span class="sxs-lookup"><span data-stu-id="d1d74-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="d1d74-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="d1d74-127">communicationError</span></span>|<span data-ttu-id="d1d74-128">19</span><span class="sxs-lookup"><span data-stu-id="d1d74-128">19</span></span>|<span data-ttu-id="d1d74-129">Der Configuration Manager-Agent konnte den Configuration Manager-Dienst in der Vergangenheit erreichen, ist aber jetzt nicht mehr in der Lage.</span><span class="sxs-lookup"><span data-stu-id="d1d74-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




