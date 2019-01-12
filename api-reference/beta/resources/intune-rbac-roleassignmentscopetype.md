---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b72e74bdb401f556214470b4c0aeda651339e332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916082"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="6246e-103">RoleAssignmentScopeType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6246e-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="6246e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6246e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6246e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6246e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6246e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6246e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6246e-107">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="6246e-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="6246e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="6246e-108">Members</span></span>
|<span data-ttu-id="6246e-109">Element</span><span class="sxs-lookup"><span data-stu-id="6246e-109">Member</span></span>|<span data-ttu-id="6246e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="6246e-110">Value</span></span>|<span data-ttu-id="6246e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6246e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6246e-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="6246e-112">resourceScope</span></span>|<span data-ttu-id="6246e-113">0</span><span class="sxs-lookup"><span data-stu-id="6246e-113">0</span></span>|<span data-ttu-id="6246e-114">Zuordnungen für den angegebenen ResourceScopes zulassen.</span><span class="sxs-lookup"><span data-stu-id="6246e-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="6246e-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="6246e-115">allDevices</span></span>|<span data-ttu-id="6246e-116">1</span><span class="sxs-lookup"><span data-stu-id="6246e-116">1</span></span>|<span data-ttu-id="6246e-117">Zuordnungen für alle Intune Geräte zulassen</span><span class="sxs-lookup"><span data-stu-id="6246e-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="6246e-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="6246e-118">allLicensedUsers</span></span>|<span data-ttu-id="6246e-119">2</span><span class="sxs-lookup"><span data-stu-id="6246e-119">2</span></span>|<span data-ttu-id="6246e-120">Zuordnungen für alle Intune lizenzierten Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="6246e-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="6246e-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="6246e-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="6246e-122">3</span><span class="sxs-lookup"><span data-stu-id="6246e-122">3</span></span>|<span data-ttu-id="6246e-123">Zuordnungen für alle Intune Geräte und lizenzierte Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="6246e-123">Allow assignments to all Intune devices and licensed users.</span></span>|





