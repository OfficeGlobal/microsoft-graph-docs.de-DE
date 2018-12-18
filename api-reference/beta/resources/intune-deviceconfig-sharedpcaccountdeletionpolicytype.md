---
title: SharedPCAccountDeletionPolicyType Enum-Typ
description: Mögliche Werte für wann Konten auf einem freigegebenen PC gelöscht werden.
author: tfitzmac
ms.openlocfilehash: 626bc7ee4006639396a7959c4f09bec47c2d7f68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335049"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="147ce-103">SharedPCAccountDeletionPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="147ce-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="147ce-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="147ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="147ce-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="147ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="147ce-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="147ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="147ce-107">Mögliche Werte für wann Konten auf einem freigegebenen PC gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="147ce-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="147ce-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="147ce-108">Members</span></span>
|<span data-ttu-id="147ce-109">Member</span><span class="sxs-lookup"><span data-stu-id="147ce-109">Member</span></span>|<span data-ttu-id="147ce-110">Wert</span><span class="sxs-lookup"><span data-stu-id="147ce-110">Value</span></span>|<span data-ttu-id="147ce-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="147ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="147ce-112">Direktfenster</span><span class="sxs-lookup"><span data-stu-id="147ce-112">immediate</span></span>|<span data-ttu-id="147ce-113">0</span><span class="sxs-lookup"><span data-stu-id="147ce-113">0</span></span>|<span data-ttu-id="147ce-114">Löschen Sie sofort.</span><span class="sxs-lookup"><span data-stu-id="147ce-114">Delete immediately.</span></span>|
|<span data-ttu-id="147ce-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="147ce-115">diskSpaceThreshold</span></span>|<span data-ttu-id="147ce-116">1</span><span class="sxs-lookup"><span data-stu-id="147ce-116">1</span></span>|<span data-ttu-id="147ce-117">Löschen Sie Disk Space Schwellenwert.</span><span class="sxs-lookup"><span data-stu-id="147ce-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="147ce-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="147ce-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="147ce-119">2</span><span class="sxs-lookup"><span data-stu-id="147ce-119">2</span></span>|<span data-ttu-id="147ce-120">Löschen Sie Disk Space Schwellenwert oder inaktiv Schwellenwert.</span><span class="sxs-lookup"><span data-stu-id="147ce-120">Delete at disk space threshold or inactive threshold.</span></span>|





