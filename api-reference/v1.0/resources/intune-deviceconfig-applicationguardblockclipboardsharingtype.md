---
title: applicationGuardBlockClipboardSharingType-Enumerationstyp
description: Mögliche Werte für applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261859"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="b1e29-103">applicationGuardBlockClipboardSharingType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="b1e29-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="b1e29-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b1e29-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1e29-105">Mögliche Werte für applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="b1e29-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="b1e29-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="b1e29-106">Members</span></span>
|<span data-ttu-id="b1e29-107">Element</span><span class="sxs-lookup"><span data-stu-id="b1e29-107">Member</span></span>|<span data-ttu-id="b1e29-108">Wert</span><span class="sxs-lookup"><span data-stu-id="b1e29-108">Value</span></span>|<span data-ttu-id="b1e29-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1e29-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1e29-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b1e29-110">notConfigured</span></span>|<span data-ttu-id="b1e29-111">0</span><span class="sxs-lookup"><span data-stu-id="b1e29-111">0</span></span>|<span data-ttu-id="b1e29-112">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="b1e29-112">Not Configured</span></span>|
|<span data-ttu-id="b1e29-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="b1e29-113">blockBoth</span></span>|<span data-ttu-id="b1e29-114">1</span><span class="sxs-lookup"><span data-stu-id="b1e29-114">1</span></span>|<span data-ttu-id="b1e29-115">Zwischenablage blockieren, um Daten von Host zu Container und von Container zu Host freizugeben</span><span class="sxs-lookup"><span data-stu-id="b1e29-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="b1e29-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="b1e29-116">blockHostToContainer</span></span>|<span data-ttu-id="b1e29-117">2</span><span class="sxs-lookup"><span data-stu-id="b1e29-117">2</span></span>|<span data-ttu-id="b1e29-118">Zwischenablage blockieren, um Daten von Host zu Container freizugeben</span><span class="sxs-lookup"><span data-stu-id="b1e29-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="b1e29-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="b1e29-119">blockContainerToHost</span></span>|<span data-ttu-id="b1e29-120">3</span><span class="sxs-lookup"><span data-stu-id="b1e29-120">3</span></span>|<span data-ttu-id="b1e29-121">Zwischenablage blockieren, um Daten von Container zu Host freizugeben</span><span class="sxs-lookup"><span data-stu-id="b1e29-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="b1e29-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="b1e29-122">blockNone</span></span>|<span data-ttu-id="b1e29-123">4</span><span class="sxs-lookup"><span data-stu-id="b1e29-123">4</span></span>|<span data-ttu-id="b1e29-124">Zwischenablage blockieren, um Daten weder vom Host-Container noch vom Container zum Host zu teilen</span><span class="sxs-lookup"><span data-stu-id="b1e29-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



