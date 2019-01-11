---
title: MacOSGatekeeperAppSources Enum-Typ
description: App-Optionen für Mac OS Gatekeeper Quelle.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6c784dba6a79b6a9d406e3632d2ac4beaf2a47ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888368"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="e69cb-103">MacOSGatekeeperAppSources Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e69cb-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="e69cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e69cb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e69cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e69cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e69cb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e69cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e69cb-107">App-Optionen für Mac OS Gatekeeper Quelle.</span><span class="sxs-lookup"><span data-stu-id="e69cb-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="e69cb-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e69cb-108">Members</span></span>
|<span data-ttu-id="e69cb-109">Element</span><span class="sxs-lookup"><span data-stu-id="e69cb-109">Member</span></span>|<span data-ttu-id="e69cb-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e69cb-110">Value</span></span>|<span data-ttu-id="e69cb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e69cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e69cb-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="e69cb-112">notConfigured</span></span>|<span data-ttu-id="e69cb-113">0</span><span class="sxs-lookup"><span data-stu-id="e69cb-113">0</span></span>|<span data-ttu-id="e69cb-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="e69cb-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e69cb-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="e69cb-115">macAppStore</span></span>|<span data-ttu-id="e69cb-116">1</span><span class="sxs-lookup"><span data-stu-id="e69cb-116">1</span></span>|<span data-ttu-id="e69cb-117">Nur apps aus der Mac-AppStore können ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e69cb-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="e69cb-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="e69cb-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="e69cb-119">2</span><span class="sxs-lookup"><span data-stu-id="e69cb-119">2</span></span>|<span data-ttu-id="e69cb-120">Nur apps aus dem Mac AppStore und identifizierten Entwickler können ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e69cb-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="e69cb-121">an einer beliebigen Stelle</span><span class="sxs-lookup"><span data-stu-id="e69cb-121">anywhere</span></span>|<span data-ttu-id="e69cb-122">3</span><span class="sxs-lookup"><span data-stu-id="e69cb-122">3</span></span>|<span data-ttu-id="e69cb-123">Apps unabhängig vom Standort können ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e69cb-123">Apps from anywhere can be run.</span></span>|





