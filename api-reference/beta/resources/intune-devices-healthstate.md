---
title: HealthState Enum-Typ
description: Gibt Integritätsstatus der Windows Management-app an.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b50023a71aaf33e2febf43e3ce96a1223eaa2ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878778"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="8e5bf-103">HealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="8e5bf-103">healthState enum type</span></span>

> <span data-ttu-id="8e5bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e5bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e5bf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e5bf-107">Gibt Integritätsstatus der Windows Management-app an.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-107">Indicates health state of the Windows management app.</span></span>
## <a name="members"></a><span data-ttu-id="8e5bf-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="8e5bf-108">Members</span></span>
|<span data-ttu-id="8e5bf-109">Element</span><span class="sxs-lookup"><span data-stu-id="8e5bf-109">Member</span></span>|<span data-ttu-id="8e5bf-110">Wert</span><span class="sxs-lookup"><span data-stu-id="8e5bf-110">Value</span></span>|<span data-ttu-id="8e5bf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e5bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e5bf-112">unknown</span><span class="sxs-lookup"><span data-stu-id="8e5bf-112">unknown</span></span>|<span data-ttu-id="8e5bf-113">0</span><span class="sxs-lookup"><span data-stu-id="8e5bf-113">0</span></span>|<span data-ttu-id="8e5bf-114">Status ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-114">Unknown state.</span></span>|
|<span data-ttu-id="8e5bf-115">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="8e5bf-115">healthy</span></span>|<span data-ttu-id="8e5bf-116">1</span><span class="sxs-lookup"><span data-stu-id="8e5bf-116">1</span></span>|<span data-ttu-id="8e5bf-117">Einem fehlerfreien Zustand.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-117">Healthy state.</span></span>|
|<span data-ttu-id="8e5bf-118">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="8e5bf-118">unhealthy</span></span>|<span data-ttu-id="8e5bf-119">2</span><span class="sxs-lookup"><span data-stu-id="8e5bf-119">2</span></span>|<span data-ttu-id="8e5bf-120">Fehlerhaften Zustand.</span><span class="sxs-lookup"><span data-stu-id="8e5bf-120">Unhealthy state.</span></span>|





