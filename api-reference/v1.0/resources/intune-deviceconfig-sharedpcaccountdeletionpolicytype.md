---
title: SharedPCAccountDeletionPolicyType Enum-Typ
description: Mögliche Werte für wann Konten auf einem freigegebenen PC gelöscht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5dc216d20becdc233bd1664250a958aa7208f1c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937628"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="55c93-103">SharedPCAccountDeletionPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="55c93-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="55c93-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="55c93-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55c93-105">Mögliche Werte für wann Konten auf einem freigegebenen PC gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="55c93-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="55c93-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="55c93-106">Members</span></span>
|<span data-ttu-id="55c93-107">Element</span><span class="sxs-lookup"><span data-stu-id="55c93-107">Member</span></span>|<span data-ttu-id="55c93-108">Wert</span><span class="sxs-lookup"><span data-stu-id="55c93-108">Value</span></span>|<span data-ttu-id="55c93-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55c93-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55c93-110">Direktfenster</span><span class="sxs-lookup"><span data-stu-id="55c93-110">immediate</span></span>|<span data-ttu-id="55c93-111">0</span><span class="sxs-lookup"><span data-stu-id="55c93-111">0</span></span>|<span data-ttu-id="55c93-112">Löschen Sie sofort.</span><span class="sxs-lookup"><span data-stu-id="55c93-112">Delete immediately.</span></span>|
|<span data-ttu-id="55c93-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="55c93-113">diskSpaceThreshold</span></span>|<span data-ttu-id="55c93-114">1</span><span class="sxs-lookup"><span data-stu-id="55c93-114">1</span></span>|<span data-ttu-id="55c93-115">Löschen Sie Disk Space Schwellenwert.</span><span class="sxs-lookup"><span data-stu-id="55c93-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="55c93-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="55c93-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="55c93-117">2</span><span class="sxs-lookup"><span data-stu-id="55c93-117">2</span></span>|<span data-ttu-id="55c93-118">Löschen Sie Disk Space Schwellenwert oder inaktiv Schwellenwert.</span><span class="sxs-lookup"><span data-stu-id="55c93-118">Delete at disk space threshold or inactive threshold.</span></span>|



