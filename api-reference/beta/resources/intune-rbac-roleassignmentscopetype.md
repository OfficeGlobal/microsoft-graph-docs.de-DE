---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
author: tfitzmac
ms.openlocfilehash: 0a3286b3b7bc583323204ca39ff85e01869ddbe7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343127"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="dbdc1-103">RoleAssignmentScopeType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="dbdc1-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="dbdc1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbdc1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbdc1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbdc1-107">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="dbdc1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="dbdc1-108">Members</span></span>
|<span data-ttu-id="dbdc1-109">Member</span><span class="sxs-lookup"><span data-stu-id="dbdc1-109">Member</span></span>|<span data-ttu-id="dbdc1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="dbdc1-110">Value</span></span>|<span data-ttu-id="dbdc1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbdc1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbdc1-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="dbdc1-112">resourceScope</span></span>|<span data-ttu-id="dbdc1-113">0</span><span class="sxs-lookup"><span data-stu-id="dbdc1-113">0</span></span>|<span data-ttu-id="dbdc1-114">Zuordnungen für den angegebenen ResourceScopes zulassen.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="dbdc1-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="dbdc1-115">allDevices</span></span>|<span data-ttu-id="dbdc1-116">1</span><span class="sxs-lookup"><span data-stu-id="dbdc1-116">1</span></span>|<span data-ttu-id="dbdc1-117">Zuordnungen für alle Intune Geräte zulassen</span><span class="sxs-lookup"><span data-stu-id="dbdc1-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="dbdc1-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="dbdc1-118">allLicensedUsers</span></span>|<span data-ttu-id="dbdc1-119">2</span><span class="sxs-lookup"><span data-stu-id="dbdc1-119">2</span></span>|<span data-ttu-id="dbdc1-120">Zuordnungen für alle Intune lizenzierten Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="dbdc1-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="dbdc1-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="dbdc1-122">3</span><span class="sxs-lookup"><span data-stu-id="dbdc1-122">3</span></span>|<span data-ttu-id="dbdc1-123">Zuordnungen für alle Intune Geräte und lizenzierte Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="dbdc1-123">Allow assignments to all Intune devices and licensed users.</span></span>|





