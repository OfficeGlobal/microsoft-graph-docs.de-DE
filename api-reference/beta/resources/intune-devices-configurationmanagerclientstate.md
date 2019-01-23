---
title: ConfigurationManagerClientState Enum-Typ
description: Konfigurations-Manager-Clientzustand
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425785"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="84066-103">ConfigurationManagerClientState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="84066-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="84066-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="84066-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84066-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84066-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84066-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84066-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84066-107">Konfigurations-Manager-Clientzustand</span><span class="sxs-lookup"><span data-stu-id="84066-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="84066-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="84066-108">Members</span></span>
|<span data-ttu-id="84066-109">Member</span><span class="sxs-lookup"><span data-stu-id="84066-109">Member</span></span>|<span data-ttu-id="84066-110">Wert</span><span class="sxs-lookup"><span data-stu-id="84066-110">Value</span></span>|<span data-ttu-id="84066-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84066-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84066-112">unknown</span><span class="sxs-lookup"><span data-stu-id="84066-112">unknown</span></span>|<span data-ttu-id="84066-113">0</span><span class="sxs-lookup"><span data-stu-id="84066-113">0</span></span>|<span data-ttu-id="84066-114">Konfigurations-Manager-Agent ist älter als 1806 oder nicht installiert oder dieses Gerät mehr als 30 Tage lang nicht in Intune eingecheckt wurde.</span><span class="sxs-lookup"><span data-stu-id="84066-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="84066-115">installiert</span><span class="sxs-lookup"><span data-stu-id="84066-115">installed</span></span>|<span data-ttu-id="84066-116">1</span><span class="sxs-lookup"><span data-stu-id="84066-116">1</span></span>|<span data-ttu-id="84066-117">Der Konfigurations-Manager-Agent ist installiert, aber möglicherweise nicht angezeigt werden Sie in der Configuration Manager-Konsole noch.</span><span class="sxs-lookup"><span data-stu-id="84066-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="84066-118">Warten Sie einige Stunden für die Aktualisierung.</span><span class="sxs-lookup"><span data-stu-id="84066-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="84066-119">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="84066-119">healthy</span></span>|<span data-ttu-id="84066-120">7</span><span class="sxs-lookup"><span data-stu-id="84066-120">7</span></span>|<span data-ttu-id="84066-121">Dieses Gerät konnte sich mit den Konfigurations-Manager-Dienst erfolgreich zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="84066-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="84066-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="84066-122">installFailed</span></span>|<span data-ttu-id="84066-123">8</span><span class="sxs-lookup"><span data-stu-id="84066-123">8</span></span>|<span data-ttu-id="84066-124">Der Konfigurations-Manager-Agent konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="84066-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="84066-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="84066-125">updateFailed</span></span>|<span data-ttu-id="84066-126">11</span><span class="sxs-lookup"><span data-stu-id="84066-126">11</span></span>|<span data-ttu-id="84066-127">Fehler beim Aktualisieren von Version X y Version der Konfigurations-Manager-Agent.</span><span class="sxs-lookup"><span data-stu-id="84066-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="84066-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="84066-128">communicationError</span></span>|<span data-ttu-id="84066-129">19</span><span class="sxs-lookup"><span data-stu-id="84066-129">19</span></span>|<span data-ttu-id="84066-130">Der Konfigurations-Manager-Agent in der Vergangenheit den Konfigurations-Manager-Dienst erreichen konnte jedoch kann jetzt nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="84066-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




