---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
ms.openlocfilehash: dcfac7b345dde2d8f107b8ec756d017966a6a94a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063364"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="31ed5-103">RoleAssignmentScopeType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="31ed5-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="31ed5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31ed5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31ed5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31ed5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31ed5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31ed5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31ed5-107">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="31ed5-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="31ed5-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="31ed5-108">Members</span></span>
|<span data-ttu-id="31ed5-109">Element</span><span class="sxs-lookup"><span data-stu-id="31ed5-109">Member</span></span>|<span data-ttu-id="31ed5-110">Wert</span><span class="sxs-lookup"><span data-stu-id="31ed5-110">Value</span></span>|<span data-ttu-id="31ed5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31ed5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ed5-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="31ed5-112">resourceScope</span></span>|<span data-ttu-id="31ed5-113">0</span><span class="sxs-lookup"><span data-stu-id="31ed5-113">0</span></span>|<span data-ttu-id="31ed5-114">Zuordnungen für den angegebenen ResourceScopes zulassen.</span><span class="sxs-lookup"><span data-stu-id="31ed5-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="31ed5-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="31ed5-115">allDevices</span></span>|<span data-ttu-id="31ed5-116">1</span><span class="sxs-lookup"><span data-stu-id="31ed5-116">1</span></span>|<span data-ttu-id="31ed5-117">Zuordnungen für alle Intune Geräte zulassen</span><span class="sxs-lookup"><span data-stu-id="31ed5-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="31ed5-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="31ed5-118">allLicensedUsers</span></span>|<span data-ttu-id="31ed5-119">2</span><span class="sxs-lookup"><span data-stu-id="31ed5-119">2</span></span>|<span data-ttu-id="31ed5-120">Zuordnungen für alle Intune lizenzierten Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="31ed5-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="31ed5-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="31ed5-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="31ed5-122">3</span><span class="sxs-lookup"><span data-stu-id="31ed5-122">3</span></span>|<span data-ttu-id="31ed5-123">Zuordnungen für alle Intune Geräte und lizenzierte Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="31ed5-123">Allow assignments to all Intune devices and licensed users.</span></span>|





