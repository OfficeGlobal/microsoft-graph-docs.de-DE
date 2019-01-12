---
title: DeviceManagementExchangeAccessState Enum-Typ
description: Exchange Access Gerätestatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a407d0971059ed7a0a8bb0ffae2773bc788b31
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928395"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="08bb7-103">DeviceManagementExchangeAccessState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="08bb7-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="08bb7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08bb7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08bb7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08bb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08bb7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="08bb7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08bb7-107">Exchange Access Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="08bb7-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="08bb7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="08bb7-108">Members</span></span>
|<span data-ttu-id="08bb7-109">Element</span><span class="sxs-lookup"><span data-stu-id="08bb7-109">Member</span></span>|<span data-ttu-id="08bb7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="08bb7-110">Value</span></span>|<span data-ttu-id="08bb7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08bb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08bb7-112">n/v</span><span class="sxs-lookup"><span data-stu-id="08bb7-112">none</span></span>|<span data-ttu-id="08bb7-113">0</span><span class="sxs-lookup"><span data-stu-id="08bb7-113">0</span></span>|<span data-ttu-id="08bb7-114">Kein Zugriff Zustand ermittelt aus Exchange</span><span class="sxs-lookup"><span data-stu-id="08bb7-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="08bb7-115">unknown</span><span class="sxs-lookup"><span data-stu-id="08bb7-115">unknown</span></span>|<span data-ttu-id="08bb7-116">1</span><span class="sxs-lookup"><span data-stu-id="08bb7-116">1</span></span>|<span data-ttu-id="08bb7-117">Access-Gerätestatus zu Exchange ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="08bb7-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="08bb7-118">zulässig</span><span class="sxs-lookup"><span data-stu-id="08bb7-118">allowed</span></span>|<span data-ttu-id="08bb7-119">2</span><span class="sxs-lookup"><span data-stu-id="08bb7-119">2</span></span>|<span data-ttu-id="08bb7-120">Das Gerät hat Zugriff auf Exchange</span><span class="sxs-lookup"><span data-stu-id="08bb7-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="08bb7-121">gesperrt</span><span class="sxs-lookup"><span data-stu-id="08bb7-121">blocked</span></span>|<span data-ttu-id="08bb7-122">3</span><span class="sxs-lookup"><span data-stu-id="08bb7-122">3</span></span>|<span data-ttu-id="08bb7-123">Gerät wird im Exchange blockiert.</span><span class="sxs-lookup"><span data-stu-id="08bb7-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="08bb7-124">unter Quarantäne gestellte e-Mails</span><span class="sxs-lookup"><span data-stu-id="08bb7-124">quarantined</span></span>|<span data-ttu-id="08bb7-125">4</span><span class="sxs-lookup"><span data-stu-id="08bb7-125">4</span></span>|<span data-ttu-id="08bb7-126">Gerät ist im Exchange unter Quarantäne gestellte e-Mails</span><span class="sxs-lookup"><span data-stu-id="08bb7-126">Device is Quarantined in Exchange</span></span>|





