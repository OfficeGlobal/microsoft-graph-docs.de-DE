---
title: ApplicationGuardBlockClipboardSharingType Enum-Typ
description: Mögliche Werte für applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7dacce6dbe91a2bbc76b52795bc20de4cf0e5f71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911882"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="79f90-103">ApplicationGuardBlockClipboardSharingType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="79f90-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="79f90-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="79f90-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79f90-105">Mögliche Werte für applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="79f90-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="79f90-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="79f90-106">Members</span></span>
|<span data-ttu-id="79f90-107">Element</span><span class="sxs-lookup"><span data-stu-id="79f90-107">Member</span></span>|<span data-ttu-id="79f90-108">Wert</span><span class="sxs-lookup"><span data-stu-id="79f90-108">Value</span></span>|<span data-ttu-id="79f90-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79f90-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f90-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="79f90-110">notConfigured</span></span>|<span data-ttu-id="79f90-111">0</span><span class="sxs-lookup"><span data-stu-id="79f90-111">0</span></span>|<span data-ttu-id="79f90-112">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="79f90-112">Not Configured</span></span>|
|<span data-ttu-id="79f90-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="79f90-113">blockBoth</span></span>|<span data-ttu-id="79f90-114">1</span><span class="sxs-lookup"><span data-stu-id="79f90-114">1</span></span>|<span data-ttu-id="79f90-115">Zwischenablage zum Freigeben von Daten aus Host Container und aus dem Container zum Hosten von blockieren</span><span class="sxs-lookup"><span data-stu-id="79f90-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="79f90-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="79f90-116">blockHostToContainer</span></span>|<span data-ttu-id="79f90-117">2</span><span class="sxs-lookup"><span data-stu-id="79f90-117">2</span></span>|<span data-ttu-id="79f90-118">Blockieren der Zwischenablage zum Freigeben von Daten vom Host Container</span><span class="sxs-lookup"><span data-stu-id="79f90-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="79f90-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="79f90-119">blockContainerToHost</span></span>|<span data-ttu-id="79f90-120">3</span><span class="sxs-lookup"><span data-stu-id="79f90-120">3</span></span>|<span data-ttu-id="79f90-121">Zwischenablage zum Freigeben von Daten aus dem Container zum Hosten von blockieren</span><span class="sxs-lookup"><span data-stu-id="79f90-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="79f90-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="79f90-122">blockNone</span></span>|<span data-ttu-id="79f90-123">4</span><span class="sxs-lookup"><span data-stu-id="79f90-123">4</span></span>|<span data-ttu-id="79f90-124">Zwischenablage zum Freigeben von Daten vom Host Container weder aus Container zum Hosten von blockieren</span><span class="sxs-lookup"><span data-stu-id="79f90-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



