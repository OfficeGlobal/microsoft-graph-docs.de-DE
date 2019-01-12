---
title: ConfigurationManagerClientState Enum-Typ
description: Konfigurations-Manager-Clientzustand
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc6f3f2db68273097d70ba9dccc6844b86afa3f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923887"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="3cfe0-103">ConfigurationManagerClientState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3cfe0-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="3cfe0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cfe0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cfe0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cfe0-107">Konfigurations-Manager-Clientzustand</span><span class="sxs-lookup"><span data-stu-id="3cfe0-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="3cfe0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3cfe0-108">Members</span></span>
|<span data-ttu-id="3cfe0-109">Element</span><span class="sxs-lookup"><span data-stu-id="3cfe0-109">Member</span></span>|<span data-ttu-id="3cfe0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3cfe0-110">Value</span></span>|<span data-ttu-id="3cfe0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cfe0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cfe0-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3cfe0-112">unknown</span></span>|<span data-ttu-id="3cfe0-113">0</span><span class="sxs-lookup"><span data-stu-id="3cfe0-113">0</span></span>|<span data-ttu-id="3cfe0-114">Konfigurations-Manager-Agent ist älter als 1806 oder nicht installiert oder dieses Gerät mehr als 30 Tage lang nicht in Intune eingecheckt wurde.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="3cfe0-115">installiert</span><span class="sxs-lookup"><span data-stu-id="3cfe0-115">installed</span></span>|<span data-ttu-id="3cfe0-116">1</span><span class="sxs-lookup"><span data-stu-id="3cfe0-116">1</span></span>|<span data-ttu-id="3cfe0-117">Der Konfigurations-Manager-Agent ist installiert, aber möglicherweise nicht angezeigt werden Sie in der Configuration Manager-Konsole noch.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="3cfe0-118">Warten Sie einige Stunden für die Aktualisierung.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="3cfe0-119">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="3cfe0-119">healthy</span></span>|<span data-ttu-id="3cfe0-120">7</span><span class="sxs-lookup"><span data-stu-id="3cfe0-120">7</span></span>|<span data-ttu-id="3cfe0-121">Dieses Gerät konnte sich mit den Konfigurations-Manager-Dienst erfolgreich zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="3cfe0-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="3cfe0-122">installFailed</span></span>|<span data-ttu-id="3cfe0-123">8</span><span class="sxs-lookup"><span data-stu-id="3cfe0-123">8</span></span>|<span data-ttu-id="3cfe0-124">Der Konfigurations-Manager-Agent konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="3cfe0-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="3cfe0-125">updateFailed</span></span>|<span data-ttu-id="3cfe0-126">11</span><span class="sxs-lookup"><span data-stu-id="3cfe0-126">11</span></span>|<span data-ttu-id="3cfe0-127">Fehler beim Aktualisieren von Version X y Version der Konfigurations-Manager-Agent.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="3cfe0-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="3cfe0-128">communicationError</span></span>|<span data-ttu-id="3cfe0-129">19</span><span class="sxs-lookup"><span data-stu-id="3cfe0-129">19</span></span>|<span data-ttu-id="3cfe0-130">Der Konfigurations-Manager-Agent in der Vergangenheit den Konfigurations-Manager-Dienst erreichen konnte jedoch kann jetzt nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="3cfe0-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





