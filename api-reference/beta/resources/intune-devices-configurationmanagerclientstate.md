---
title: ConfigurationManagerClientState Enum-Typ
description: Konfigurations-Manager-Clientzustand
author: tfitzmac
ms.openlocfilehash: dc67a5fb1c517e65da937996ed65adaa621fa3c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354047"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="0f5f9-103">ConfigurationManagerClientState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0f5f9-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="0f5f9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f5f9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f5f9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f5f9-107">Konfigurations-Manager-Clientzustand</span><span class="sxs-lookup"><span data-stu-id="0f5f9-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="0f5f9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0f5f9-108">Members</span></span>
|<span data-ttu-id="0f5f9-109">Member</span><span class="sxs-lookup"><span data-stu-id="0f5f9-109">Member</span></span>|<span data-ttu-id="0f5f9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0f5f9-110">Value</span></span>|<span data-ttu-id="0f5f9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f5f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f5f9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="0f5f9-112">unknown</span></span>|<span data-ttu-id="0f5f9-113">0</span><span class="sxs-lookup"><span data-stu-id="0f5f9-113">0</span></span>|<span data-ttu-id="0f5f9-114">Konfigurations-Manager-Agent ist älter als 1806 oder nicht installiert oder dieses Gerät mehr als 30 Tage lang nicht in Intune eingecheckt wurde.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="0f5f9-115">installiert</span><span class="sxs-lookup"><span data-stu-id="0f5f9-115">installed</span></span>|<span data-ttu-id="0f5f9-116">1</span><span class="sxs-lookup"><span data-stu-id="0f5f9-116">1</span></span>|<span data-ttu-id="0f5f9-117">Der Konfigurations-Manager-Agent ist installiert, aber möglicherweise nicht angezeigt werden Sie in der Configuration Manager-Konsole noch.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="0f5f9-118">Warten Sie einige Stunden für die Aktualisierung.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="0f5f9-119">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="0f5f9-119">healthy</span></span>|<span data-ttu-id="0f5f9-120">7</span><span class="sxs-lookup"><span data-stu-id="0f5f9-120">7</span></span>|<span data-ttu-id="0f5f9-121">Dieses Gerät konnte sich mit den Konfigurations-Manager-Dienst erfolgreich zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="0f5f9-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="0f5f9-122">installFailed</span></span>|<span data-ttu-id="0f5f9-123">8</span><span class="sxs-lookup"><span data-stu-id="0f5f9-123">8</span></span>|<span data-ttu-id="0f5f9-124">Der Konfigurations-Manager-Agent konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="0f5f9-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="0f5f9-125">updateFailed</span></span>|<span data-ttu-id="0f5f9-126">11</span><span class="sxs-lookup"><span data-stu-id="0f5f9-126">11</span></span>|<span data-ttu-id="0f5f9-127">Fehler beim Aktualisieren von Version X y Version der Konfigurations-Manager-Agent.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="0f5f9-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="0f5f9-128">communicationError</span></span>|<span data-ttu-id="0f5f9-129">19</span><span class="sxs-lookup"><span data-stu-id="0f5f9-129">19</span></span>|<span data-ttu-id="0f5f9-130">Der Konfigurations-Manager-Agent in der Vergangenheit den Konfigurations-Manager-Dienst erreichen konnte jedoch kann jetzt nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="0f5f9-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





