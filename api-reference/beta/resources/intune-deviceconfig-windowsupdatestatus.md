---
title: windowsUpdateStatus-Enumerationstyp
description: Windows Update for Business-Konfigurations Gerätestatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7549fb77cf5a9f7c3014192d5524019323405f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154159"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="1bb3c-103">windowsUpdateStatus-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="1bb3c-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="1bb3c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bb3c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bb3c-106">Windows Update for Business-Konfigurations Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="1bb3c-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="1bb3c-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1bb3c-107">Members</span></span>
|<span data-ttu-id="1bb3c-108">Element</span><span class="sxs-lookup"><span data-stu-id="1bb3c-108">Member</span></span>|<span data-ttu-id="1bb3c-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1bb3c-109">Value</span></span>|<span data-ttu-id="1bb3c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1bb3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bb3c-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="1bb3c-111">upToDate</span></span>|<span data-ttu-id="1bb3c-112">0</span><span class="sxs-lookup"><span data-stu-id="1bb3c-112">0</span></span>|<span data-ttu-id="1bb3c-113">Es sind keine Updates, keine ausstehenden Neustart Updates und keine fehlerhaften Updates vorhanden.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="1bb3c-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="1bb3c-114">pendingInstallation</span></span>|<span data-ttu-id="1bb3c-115">1</span><span class="sxs-lookup"><span data-stu-id="1bb3c-115">1</span></span>|<span data-ttu-id="1bb3c-116">Es gibt Updates für die Installation, die nicht genehmigte Updates enthalten.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="1bb3c-117">Es sind keine Updates für den Neustart vorhanden, keine fehlerhaften Aktualisierungen.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="1bb3c-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="1bb3c-118">pendingReboot</span></span>|<span data-ttu-id="1bb3c-119">2</span><span class="sxs-lookup"><span data-stu-id="1bb3c-119">2</span></span>|<span data-ttu-id="1bb3c-120">Es gibt Updates, die einen Neustart erfordern.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-120">There are updates that requires reboot.</span></span> <span data-ttu-id="1bb3c-121">Es sind keine fehlerhaften Aktualisierungen vorhanden.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-121">There are not failed updates.</span></span>|
|<span data-ttu-id="1bb3c-122">failed</span><span class="sxs-lookup"><span data-stu-id="1bb3c-122">failed</span></span>|<span data-ttu-id="1bb3c-123">3</span><span class="sxs-lookup"><span data-stu-id="1bb3c-123">3</span></span>|<span data-ttu-id="1bb3c-124">Es sind keine Updates auf dem Gerät installiert.</span><span class="sxs-lookup"><span data-stu-id="1bb3c-124">There are updates failed to install on the device.</span></span>|




