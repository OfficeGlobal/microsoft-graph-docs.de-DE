---
title: DeviceManagementExchangeAccessState Enum-Typ
description: Exchange Access Gerätestatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b6d831eb226648dcdbdbe470c82df900a8464a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817844"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="cc8b1-103">DeviceManagementExchangeAccessState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cc8b1-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="cc8b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cc8b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc8b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cc8b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc8b1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cc8b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc8b1-107">Exchange Access Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="cc8b1-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="cc8b1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="cc8b1-108">Members</span></span>
|<span data-ttu-id="cc8b1-109">Element</span><span class="sxs-lookup"><span data-stu-id="cc8b1-109">Member</span></span>|<span data-ttu-id="cc8b1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="cc8b1-110">Value</span></span>|<span data-ttu-id="cc8b1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc8b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8b1-112">n/v</span><span class="sxs-lookup"><span data-stu-id="cc8b1-112">none</span></span>|<span data-ttu-id="cc8b1-113">0</span><span class="sxs-lookup"><span data-stu-id="cc8b1-113">0</span></span>|<span data-ttu-id="cc8b1-114">Kein Zugriff Zustand ermittelt aus Exchange</span><span class="sxs-lookup"><span data-stu-id="cc8b1-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="cc8b1-115">unknown</span><span class="sxs-lookup"><span data-stu-id="cc8b1-115">unknown</span></span>|<span data-ttu-id="cc8b1-116">1</span><span class="sxs-lookup"><span data-stu-id="cc8b1-116">1</span></span>|<span data-ttu-id="cc8b1-117">Access-Gerätestatus zu Exchange ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="cc8b1-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="cc8b1-118">zulässig</span><span class="sxs-lookup"><span data-stu-id="cc8b1-118">allowed</span></span>|<span data-ttu-id="cc8b1-119">2</span><span class="sxs-lookup"><span data-stu-id="cc8b1-119">2</span></span>|<span data-ttu-id="cc8b1-120">Das Gerät hat Zugriff auf Exchange</span><span class="sxs-lookup"><span data-stu-id="cc8b1-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="cc8b1-121">gesperrt</span><span class="sxs-lookup"><span data-stu-id="cc8b1-121">blocked</span></span>|<span data-ttu-id="cc8b1-122">3</span><span class="sxs-lookup"><span data-stu-id="cc8b1-122">3</span></span>|<span data-ttu-id="cc8b1-123">Gerät wird im Exchange blockiert.</span><span class="sxs-lookup"><span data-stu-id="cc8b1-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="cc8b1-124">unter Quarantäne gestellte e-Mails</span><span class="sxs-lookup"><span data-stu-id="cc8b1-124">quarantined</span></span>|<span data-ttu-id="cc8b1-125">4</span><span class="sxs-lookup"><span data-stu-id="cc8b1-125">4</span></span>|<span data-ttu-id="cc8b1-126">Gerät ist im Exchange unter Quarantäne gestellte e-Mails</span><span class="sxs-lookup"><span data-stu-id="cc8b1-126">Device is Quarantined in Exchange</span></span>|





