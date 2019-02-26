---
title: vppTokenState-Enumerationstyp
description: Mögliche Status, die einem Apple Volume Purchase Program-Token zugeordnet sind.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254933"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="45baa-103">vppTokenState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="45baa-103">vppTokenState enum type</span></span>

> <span data-ttu-id="45baa-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="45baa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45baa-105">Mögliche Status, die einem Apple Volume Purchase Program-Token zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="45baa-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="45baa-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="45baa-106">Members</span></span>
|<span data-ttu-id="45baa-107">Element</span><span class="sxs-lookup"><span data-stu-id="45baa-107">Member</span></span>|<span data-ttu-id="45baa-108">Wert</span><span class="sxs-lookup"><span data-stu-id="45baa-108">Value</span></span>|<span data-ttu-id="45baa-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45baa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45baa-110">unknown</span><span class="sxs-lookup"><span data-stu-id="45baa-110">unknown</span></span>|<span data-ttu-id="45baa-111">0</span><span class="sxs-lookup"><span data-stu-id="45baa-111">0</span></span>|<span data-ttu-id="45baa-112">Standardzustand.</span><span class="sxs-lookup"><span data-stu-id="45baa-112">Default state.</span></span>|
|<span data-ttu-id="45baa-113">gültige</span><span class="sxs-lookup"><span data-stu-id="45baa-113">valid</span></span>|<span data-ttu-id="45baa-114">1</span><span class="sxs-lookup"><span data-stu-id="45baa-114">1</span></span>|<span data-ttu-id="45baa-115">Token ist gültig.</span><span class="sxs-lookup"><span data-stu-id="45baa-115">Token is valid.</span></span>|
|<span data-ttu-id="45baa-116">abgelaufen</span><span class="sxs-lookup"><span data-stu-id="45baa-116">expired</span></span>|<span data-ttu-id="45baa-117">2</span><span class="sxs-lookup"><span data-stu-id="45baa-117">2</span></span>|<span data-ttu-id="45baa-118">Token ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="45baa-118">Token is expired.</span></span>|
|<span data-ttu-id="45baa-119">Ungültig</span><span class="sxs-lookup"><span data-stu-id="45baa-119">invalid</span></span>|<span data-ttu-id="45baa-120">3</span><span class="sxs-lookup"><span data-stu-id="45baa-120">3</span></span>|<span data-ttu-id="45baa-121">Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="45baa-121">Token is invalid.</span></span>|
|<span data-ttu-id="45baa-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="45baa-122">assignedToExternalMDM</span></span>|<span data-ttu-id="45baa-123">4</span><span class="sxs-lookup"><span data-stu-id="45baa-123">4</span></span>|<span data-ttu-id="45baa-124">Token wird von einem anderen MDM-Dienst verwaltet.</span><span class="sxs-lookup"><span data-stu-id="45baa-124">Token is managed by another MDM Service.</span></span>|



