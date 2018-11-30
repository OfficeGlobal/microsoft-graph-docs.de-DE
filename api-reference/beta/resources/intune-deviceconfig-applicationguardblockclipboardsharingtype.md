---
title: ApplicationGuardBlockClipboardSharingType Enum-Typ
description: Mögliche Werte für applicationGuardBlockClipboardSharingType
ms.openlocfilehash: e0e05001e4f3cedc2893fc6b2006f5b5b5d74db6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062560"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="5af52-103">ApplicationGuardBlockClipboardSharingType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5af52-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="5af52-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5af52-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5af52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5af52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5af52-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5af52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5af52-107">Mögliche Werte für applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="5af52-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="5af52-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5af52-108">Members</span></span>
|<span data-ttu-id="5af52-109">Element</span><span class="sxs-lookup"><span data-stu-id="5af52-109">Member</span></span>|<span data-ttu-id="5af52-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5af52-110">Value</span></span>|<span data-ttu-id="5af52-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5af52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af52-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="5af52-112">notConfigured</span></span>|<span data-ttu-id="5af52-113">0</span><span class="sxs-lookup"><span data-stu-id="5af52-113">0</span></span>|<span data-ttu-id="5af52-114">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="5af52-114">Not Configured</span></span>|
|<span data-ttu-id="5af52-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="5af52-115">blockBoth</span></span>|<span data-ttu-id="5af52-116">1</span><span class="sxs-lookup"><span data-stu-id="5af52-116">1</span></span>|<span data-ttu-id="5af52-117">Zwischenablage zum Freigeben von Daten aus Host Container und aus dem Container zum Hosten von blockieren</span><span class="sxs-lookup"><span data-stu-id="5af52-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="5af52-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="5af52-118">blockHostToContainer</span></span>|<span data-ttu-id="5af52-119">2</span><span class="sxs-lookup"><span data-stu-id="5af52-119">2</span></span>|<span data-ttu-id="5af52-120">Blockieren der Zwischenablage zum Freigeben von Daten vom Host Container</span><span class="sxs-lookup"><span data-stu-id="5af52-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="5af52-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="5af52-121">blockContainerToHost</span></span>|<span data-ttu-id="5af52-122">3</span><span class="sxs-lookup"><span data-stu-id="5af52-122">3</span></span>|<span data-ttu-id="5af52-123">Zwischenablage zum Freigeben von Daten aus dem Container zum Hosten von blockieren</span><span class="sxs-lookup"><span data-stu-id="5af52-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="5af52-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="5af52-124">blockNone</span></span>|<span data-ttu-id="5af52-125">4</span><span class="sxs-lookup"><span data-stu-id="5af52-125">4</span></span>|<span data-ttu-id="5af52-126">Zwischenablage zum Freigeben von Daten vom Host Container weder aus Container zum Hosten von blockieren</span><span class="sxs-lookup"><span data-stu-id="5af52-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





