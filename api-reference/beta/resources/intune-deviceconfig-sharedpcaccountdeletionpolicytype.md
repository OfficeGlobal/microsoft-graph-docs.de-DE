---
title: SharedPCAccountDeletionPolicyType Enum-Typ
description: Mögliche Werte für wann Konten auf einem freigegebenen PC gelöscht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 081069f9462c426f24a1e3cf276730b1db40b191
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951950"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="7a2ad-103">SharedPCAccountDeletionPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7a2ad-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="7a2ad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a2ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a2ad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a2ad-107">Mögliche Werte für wann Konten auf einem freigegebenen PC gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="7a2ad-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="7a2ad-108">Members</span></span>
|<span data-ttu-id="7a2ad-109">Element</span><span class="sxs-lookup"><span data-stu-id="7a2ad-109">Member</span></span>|<span data-ttu-id="7a2ad-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7a2ad-110">Value</span></span>|<span data-ttu-id="7a2ad-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a2ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a2ad-112">Direktfenster</span><span class="sxs-lookup"><span data-stu-id="7a2ad-112">immediate</span></span>|<span data-ttu-id="7a2ad-113">0</span><span class="sxs-lookup"><span data-stu-id="7a2ad-113">0</span></span>|<span data-ttu-id="7a2ad-114">Löschen Sie sofort.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-114">Delete immediately.</span></span>|
|<span data-ttu-id="7a2ad-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="7a2ad-115">diskSpaceThreshold</span></span>|<span data-ttu-id="7a2ad-116">1</span><span class="sxs-lookup"><span data-stu-id="7a2ad-116">1</span></span>|<span data-ttu-id="7a2ad-117">Löschen Sie Disk Space Schwellenwert.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="7a2ad-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="7a2ad-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="7a2ad-119">2</span><span class="sxs-lookup"><span data-stu-id="7a2ad-119">2</span></span>|<span data-ttu-id="7a2ad-120">Löschen Sie Disk Space Schwellenwert oder inaktiv Schwellenwert.</span><span class="sxs-lookup"><span data-stu-id="7a2ad-120">Delete at disk space threshold or inactive threshold.</span></span>|





