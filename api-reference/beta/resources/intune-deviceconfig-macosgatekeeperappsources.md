---
title: MacOSGatekeeperAppSources Enum-Typ
description: App-Optionen für Mac OS Gatekeeper Quelle.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c2c1d553408b7269a53f9fc3500493a44bc3645
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918114"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="961c9-103">MacOSGatekeeperAppSources Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="961c9-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="961c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="961c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="961c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="961c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="961c9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="961c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="961c9-107">App-Optionen für Mac OS Gatekeeper Quelle.</span><span class="sxs-lookup"><span data-stu-id="961c9-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="961c9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="961c9-108">Members</span></span>
|<span data-ttu-id="961c9-109">Element</span><span class="sxs-lookup"><span data-stu-id="961c9-109">Member</span></span>|<span data-ttu-id="961c9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="961c9-110">Value</span></span>|<span data-ttu-id="961c9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="961c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="961c9-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="961c9-112">notConfigured</span></span>|<span data-ttu-id="961c9-113">0</span><span class="sxs-lookup"><span data-stu-id="961c9-113">0</span></span>|<span data-ttu-id="961c9-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="961c9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="961c9-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="961c9-115">macAppStore</span></span>|<span data-ttu-id="961c9-116">1</span><span class="sxs-lookup"><span data-stu-id="961c9-116">1</span></span>|<span data-ttu-id="961c9-117">Nur apps aus der Mac-AppStore können ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="961c9-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="961c9-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="961c9-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="961c9-119">2</span><span class="sxs-lookup"><span data-stu-id="961c9-119">2</span></span>|<span data-ttu-id="961c9-120">Nur apps aus dem Mac AppStore und identifizierten Entwickler können ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="961c9-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="961c9-121">an einer beliebigen Stelle</span><span class="sxs-lookup"><span data-stu-id="961c9-121">anywhere</span></span>|<span data-ttu-id="961c9-122">3</span><span class="sxs-lookup"><span data-stu-id="961c9-122">3</span></span>|<span data-ttu-id="961c9-123">Apps unabhängig vom Standort können ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="961c9-123">Apps from anywhere can be run.</span></span>|





