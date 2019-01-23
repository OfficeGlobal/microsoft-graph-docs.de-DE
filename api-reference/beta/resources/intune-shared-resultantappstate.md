---
title: ResultantAppState Enum-Typ
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf3d7e8ef20b1458811ae1a49b23120f7cd153d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422684"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="64275-103">ResultantAppState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="64275-103">resultantAppState enum type</span></span>

> <span data-ttu-id="64275-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="64275-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64275-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64275-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64275-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64275-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64275-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="64275-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="64275-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="64275-108">Members</span></span>
|<span data-ttu-id="64275-109">Member</span><span class="sxs-lookup"><span data-stu-id="64275-109">Member</span></span>|<span data-ttu-id="64275-110">Wert</span><span class="sxs-lookup"><span data-stu-id="64275-110">Value</span></span>|<span data-ttu-id="64275-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64275-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64275-112">installiert</span><span class="sxs-lookup"><span data-stu-id="64275-112">installed</span></span>|<span data-ttu-id="64275-113">1</span><span class="sxs-lookup"><span data-stu-id="64275-113">1</span></span>|<span data-ttu-id="64275-114">Die Anwendung wird ohne Fehler installiert.</span><span class="sxs-lookup"><span data-stu-id="64275-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="64275-115">failed</span><span class="sxs-lookup"><span data-stu-id="64275-115">failed</span></span>|<span data-ttu-id="64275-116">2</span><span class="sxs-lookup"><span data-stu-id="64275-116">2</span></span>|<span data-ttu-id="64275-117">Die Anwendung konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="64275-117">The application failed to install.</span></span>|
|<span data-ttu-id="64275-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="64275-118">notInstalled</span></span>|<span data-ttu-id="64275-119">3</span><span class="sxs-lookup"><span data-stu-id="64275-119">3</span></span>|<span data-ttu-id="64275-120">Die Anwendung ist nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="64275-120">The application is not installed.</span></span>|
|<span data-ttu-id="64275-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="64275-121">uninstallFailed</span></span>|<span data-ttu-id="64275-122">4</span><span class="sxs-lookup"><span data-stu-id="64275-122">4</span></span>|<span data-ttu-id="64275-123">Die Anwendung konnte nicht deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="64275-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="64275-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="64275-124">pendingInstall</span></span>|<span data-ttu-id="64275-125">5</span><span class="sxs-lookup"><span data-stu-id="64275-125">5</span></span>|<span data-ttu-id="64275-126">Die Installation der Anwendung wird gerade durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="64275-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="64275-127">unknown</span><span class="sxs-lookup"><span data-stu-id="64275-127">unknown</span></span>|<span data-ttu-id="64275-128">99</span><span class="sxs-lookup"><span data-stu-id="64275-128">99</span></span>|<span data-ttu-id="64275-129">Der Status der Anwendung ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="64275-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="64275-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="64275-130">notApplicable</span></span>|<span data-ttu-id="64275-131">-1</span><span class="sxs-lookup"><span data-stu-id="64275-131">-1</span></span>|<span data-ttu-id="64275-132">Die Anwendung ist nicht anwendbar.</span><span class="sxs-lookup"><span data-stu-id="64275-132">The application is not applicable.</span></span>|




