---
title: VppTokenState Enum-Typ
description: Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d0c4ee7ae0b8e35f97a18d0958a2456cab40a10
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416160"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="67ca1-103">VppTokenState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="67ca1-103">vppTokenState enum type</span></span>

> <span data-ttu-id="67ca1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="67ca1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67ca1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67ca1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67ca1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67ca1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67ca1-107">Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="67ca1-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="67ca1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="67ca1-108">Members</span></span>
|<span data-ttu-id="67ca1-109">Member</span><span class="sxs-lookup"><span data-stu-id="67ca1-109">Member</span></span>|<span data-ttu-id="67ca1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="67ca1-110">Value</span></span>|<span data-ttu-id="67ca1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67ca1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67ca1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="67ca1-112">unknown</span></span>|<span data-ttu-id="67ca1-113">0</span><span class="sxs-lookup"><span data-stu-id="67ca1-113">0</span></span>|<span data-ttu-id="67ca1-114">Standardzustand.</span><span class="sxs-lookup"><span data-stu-id="67ca1-114">Default state.</span></span>|
|<span data-ttu-id="67ca1-115">gültige</span><span class="sxs-lookup"><span data-stu-id="67ca1-115">valid</span></span>|<span data-ttu-id="67ca1-116">1</span><span class="sxs-lookup"><span data-stu-id="67ca1-116">1</span></span>|<span data-ttu-id="67ca1-117">Das Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="67ca1-117">Token is valid.</span></span>|
|<span data-ttu-id="67ca1-118">abgelaufen</span><span class="sxs-lookup"><span data-stu-id="67ca1-118">expired</span></span>|<span data-ttu-id="67ca1-119">2</span><span class="sxs-lookup"><span data-stu-id="67ca1-119">2</span></span>|<span data-ttu-id="67ca1-120">Token ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="67ca1-120">Token is expired.</span></span>|
|<span data-ttu-id="67ca1-121">Ungültig</span><span class="sxs-lookup"><span data-stu-id="67ca1-121">invalid</span></span>|<span data-ttu-id="67ca1-122">3</span><span class="sxs-lookup"><span data-stu-id="67ca1-122">3</span></span>|<span data-ttu-id="67ca1-123">Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="67ca1-123">Token is invalid.</span></span>|
|<span data-ttu-id="67ca1-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="67ca1-124">assignedToExternalMDM</span></span>|<span data-ttu-id="67ca1-125">4</span><span class="sxs-lookup"><span data-stu-id="67ca1-125">4</span></span>|<span data-ttu-id="67ca1-126">Token wird von einem anderen MDM-Dienst verwaltet.</span><span class="sxs-lookup"><span data-stu-id="67ca1-126">Token is managed by another MDM Service.</span></span>|




