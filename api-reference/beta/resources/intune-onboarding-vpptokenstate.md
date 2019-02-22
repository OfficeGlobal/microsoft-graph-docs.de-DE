---
title: vppTokenState-Enumerationstyp
description: Mögliche Status, die einem Apple Volume Purchase Program-Token zugeordnet sind.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdb356d5103fc1c1dc07245d8552cb77b9383c8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159864"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="af037-103">vppTokenState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="af037-103">vppTokenState enum type</span></span>

> <span data-ttu-id="af037-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af037-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af037-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="af037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af037-106">Mögliche Status, die einem Apple Volume Purchase Program-Token zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="af037-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="af037-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="af037-107">Members</span></span>
|<span data-ttu-id="af037-108">Element</span><span class="sxs-lookup"><span data-stu-id="af037-108">Member</span></span>|<span data-ttu-id="af037-109">Wert</span><span class="sxs-lookup"><span data-stu-id="af037-109">Value</span></span>|<span data-ttu-id="af037-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af037-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af037-111">unknown</span><span class="sxs-lookup"><span data-stu-id="af037-111">unknown</span></span>|<span data-ttu-id="af037-112">0</span><span class="sxs-lookup"><span data-stu-id="af037-112">0</span></span>|<span data-ttu-id="af037-113">Standardzustand.</span><span class="sxs-lookup"><span data-stu-id="af037-113">Default state.</span></span>|
|<span data-ttu-id="af037-114">gültige</span><span class="sxs-lookup"><span data-stu-id="af037-114">valid</span></span>|<span data-ttu-id="af037-115">1</span><span class="sxs-lookup"><span data-stu-id="af037-115">1</span></span>|<span data-ttu-id="af037-116">Token ist gültig.</span><span class="sxs-lookup"><span data-stu-id="af037-116">Token is valid.</span></span>|
|<span data-ttu-id="af037-117">abgelaufen</span><span class="sxs-lookup"><span data-stu-id="af037-117">expired</span></span>|<span data-ttu-id="af037-118">2</span><span class="sxs-lookup"><span data-stu-id="af037-118">2</span></span>|<span data-ttu-id="af037-119">Token ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="af037-119">Token is expired.</span></span>|
|<span data-ttu-id="af037-120">Ungültig</span><span class="sxs-lookup"><span data-stu-id="af037-120">invalid</span></span>|<span data-ttu-id="af037-121">3</span><span class="sxs-lookup"><span data-stu-id="af037-121">3</span></span>|<span data-ttu-id="af037-122">Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="af037-122">Token is invalid.</span></span>|
|<span data-ttu-id="af037-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="af037-123">assignedToExternalMDM</span></span>|<span data-ttu-id="af037-124">4</span><span class="sxs-lookup"><span data-stu-id="af037-124">4</span></span>|<span data-ttu-id="af037-125">Token wird von einem anderen MDM-Dienst verwaltet.</span><span class="sxs-lookup"><span data-stu-id="af037-125">Token is managed by another MDM Service.</span></span>|




