---
title: ConfigurationManagerClientState Enum-Typ
description: Konfigurations-Manager-Clientzustand
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 36abbe4451a6e053387b27fce3e9a4e25dcc1a95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806251"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="88462-103">ConfigurationManagerClientState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="88462-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="88462-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="88462-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88462-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88462-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88462-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="88462-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88462-107">Konfigurations-Manager-Clientzustand</span><span class="sxs-lookup"><span data-stu-id="88462-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="88462-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="88462-108">Members</span></span>
|<span data-ttu-id="88462-109">Element</span><span class="sxs-lookup"><span data-stu-id="88462-109">Member</span></span>|<span data-ttu-id="88462-110">Wert</span><span class="sxs-lookup"><span data-stu-id="88462-110">Value</span></span>|<span data-ttu-id="88462-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88462-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88462-112">unknown</span><span class="sxs-lookup"><span data-stu-id="88462-112">unknown</span></span>|<span data-ttu-id="88462-113">0</span><span class="sxs-lookup"><span data-stu-id="88462-113">0</span></span>|<span data-ttu-id="88462-114">Konfigurations-Manager-Agent ist älter als 1806 oder nicht installiert oder dieses Gerät mehr als 30 Tage lang nicht in Intune eingecheckt wurde.</span><span class="sxs-lookup"><span data-stu-id="88462-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="88462-115">installiert</span><span class="sxs-lookup"><span data-stu-id="88462-115">installed</span></span>|<span data-ttu-id="88462-116">1</span><span class="sxs-lookup"><span data-stu-id="88462-116">1</span></span>|<span data-ttu-id="88462-117">Der Konfigurations-Manager-Agent ist installiert, aber möglicherweise nicht angezeigt werden Sie in der Configuration Manager-Konsole noch.</span><span class="sxs-lookup"><span data-stu-id="88462-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="88462-118">Warten Sie einige Stunden für die Aktualisierung.</span><span class="sxs-lookup"><span data-stu-id="88462-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="88462-119">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="88462-119">healthy</span></span>|<span data-ttu-id="88462-120">7</span><span class="sxs-lookup"><span data-stu-id="88462-120">7</span></span>|<span data-ttu-id="88462-121">Dieses Gerät konnte sich mit den Konfigurations-Manager-Dienst erfolgreich zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="88462-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="88462-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="88462-122">installFailed</span></span>|<span data-ttu-id="88462-123">8</span><span class="sxs-lookup"><span data-stu-id="88462-123">8</span></span>|<span data-ttu-id="88462-124">Der Konfigurations-Manager-Agent konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="88462-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="88462-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="88462-125">updateFailed</span></span>|<span data-ttu-id="88462-126">11</span><span class="sxs-lookup"><span data-stu-id="88462-126">11</span></span>|<span data-ttu-id="88462-127">Fehler beim Aktualisieren von Version X y Version der Konfigurations-Manager-Agent.</span><span class="sxs-lookup"><span data-stu-id="88462-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="88462-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="88462-128">communicationError</span></span>|<span data-ttu-id="88462-129">19</span><span class="sxs-lookup"><span data-stu-id="88462-129">19</span></span>|<span data-ttu-id="88462-130">Der Konfigurations-Manager-Agent in der Vergangenheit den Konfigurations-Manager-Dienst erreichen konnte jedoch kann jetzt nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="88462-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





