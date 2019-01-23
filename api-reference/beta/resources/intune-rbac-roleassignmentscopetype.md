---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419891"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="f5ac7-103">RoleAssignmentScopeType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f5ac7-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="f5ac7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5ac7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5ac7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ac7-107">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="f5ac7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f5ac7-108">Members</span></span>
|<span data-ttu-id="f5ac7-109">Member</span><span class="sxs-lookup"><span data-stu-id="f5ac7-109">Member</span></span>|<span data-ttu-id="f5ac7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f5ac7-110">Value</span></span>|<span data-ttu-id="f5ac7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5ac7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ac7-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="f5ac7-112">resourceScope</span></span>|<span data-ttu-id="f5ac7-113">0</span><span class="sxs-lookup"><span data-stu-id="f5ac7-113">0</span></span>|<span data-ttu-id="f5ac7-114">Zuordnungen für den angegebenen ResourceScopes zulassen.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="f5ac7-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="f5ac7-115">allDevices</span></span>|<span data-ttu-id="f5ac7-116">1</span><span class="sxs-lookup"><span data-stu-id="f5ac7-116">1</span></span>|<span data-ttu-id="f5ac7-117">Zuordnungen für alle Intune Geräte zulassen</span><span class="sxs-lookup"><span data-stu-id="f5ac7-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="f5ac7-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="f5ac7-118">allLicensedUsers</span></span>|<span data-ttu-id="f5ac7-119">2</span><span class="sxs-lookup"><span data-stu-id="f5ac7-119">2</span></span>|<span data-ttu-id="f5ac7-120">Zuordnungen für alle Intune lizenzierten Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="f5ac7-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="f5ac7-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="f5ac7-122">3</span><span class="sxs-lookup"><span data-stu-id="f5ac7-122">3</span></span>|<span data-ttu-id="f5ac7-123">Zuordnungen für alle Intune Geräte und lizenzierte Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-123">Allow assignments to all Intune devices and licensed users.</span></span>|




