---
title: applicationGuardBlockClipboardSharingType-Enumerationstyp
description: Mögliche Werte für applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dba5ba1a2d27862c9adaaa1430631b8cb4cf94d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160662"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="bf968-103">applicationGuardBlockClipboardSharingType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="bf968-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="bf968-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf968-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf968-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bf968-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf968-106">Mögliche Werte für applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="bf968-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="bf968-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="bf968-107">Members</span></span>
|<span data-ttu-id="bf968-108">Element</span><span class="sxs-lookup"><span data-stu-id="bf968-108">Member</span></span>|<span data-ttu-id="bf968-109">Wert</span><span class="sxs-lookup"><span data-stu-id="bf968-109">Value</span></span>|<span data-ttu-id="bf968-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf968-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf968-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bf968-111">notConfigured</span></span>|<span data-ttu-id="bf968-112">0</span><span class="sxs-lookup"><span data-stu-id="bf968-112">0</span></span>|<span data-ttu-id="bf968-113">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="bf968-113">Not Configured</span></span>|
|<span data-ttu-id="bf968-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="bf968-114">blockBoth</span></span>|<span data-ttu-id="bf968-115">1</span><span class="sxs-lookup"><span data-stu-id="bf968-115">1</span></span>|<span data-ttu-id="bf968-116">Zwischenablage blockieren, um Daten von Host zu Container und von Container zu Host freizugeben</span><span class="sxs-lookup"><span data-stu-id="bf968-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="bf968-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="bf968-117">blockHostToContainer</span></span>|<span data-ttu-id="bf968-118">2</span><span class="sxs-lookup"><span data-stu-id="bf968-118">2</span></span>|<span data-ttu-id="bf968-119">Zwischenablage blockieren, um Daten von Host zu Container freizugeben</span><span class="sxs-lookup"><span data-stu-id="bf968-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="bf968-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="bf968-120">blockContainerToHost</span></span>|<span data-ttu-id="bf968-121">3</span><span class="sxs-lookup"><span data-stu-id="bf968-121">3</span></span>|<span data-ttu-id="bf968-122">Zwischenablage blockieren, um Daten von Container zu Host freizugeben</span><span class="sxs-lookup"><span data-stu-id="bf968-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="bf968-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="bf968-123">blockNone</span></span>|<span data-ttu-id="bf968-124">4</span><span class="sxs-lookup"><span data-stu-id="bf968-124">4</span></span>|<span data-ttu-id="bf968-125">Zwischenablage blockieren, um Daten weder vom Host-Container noch vom Container zum Host zu teilen</span><span class="sxs-lookup"><span data-stu-id="bf968-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




