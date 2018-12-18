---
title: HealthState Enum-Typ
description: Gibt Integritätsstatus der Windows Management-app an.
author: tfitzmac
ms.openlocfilehash: 831caf85b5beb4c90721aea44054b85d64817c84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308722"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="1801e-103">HealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1801e-103">healthState enum type</span></span>

> <span data-ttu-id="1801e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1801e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1801e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1801e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1801e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1801e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1801e-107">Gibt Integritätsstatus der Windows Management-app an.</span><span class="sxs-lookup"><span data-stu-id="1801e-107">Indicates health state of the Windows management app.</span></span>
## <a name="members"></a><span data-ttu-id="1801e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1801e-108">Members</span></span>
|<span data-ttu-id="1801e-109">Member</span><span class="sxs-lookup"><span data-stu-id="1801e-109">Member</span></span>|<span data-ttu-id="1801e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1801e-110">Value</span></span>|<span data-ttu-id="1801e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1801e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1801e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1801e-112">unknown</span></span>|<span data-ttu-id="1801e-113">0</span><span class="sxs-lookup"><span data-stu-id="1801e-113">0</span></span>|<span data-ttu-id="1801e-114">Status ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="1801e-114">Unknown state.</span></span>|
|<span data-ttu-id="1801e-115">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="1801e-115">healthy</span></span>|<span data-ttu-id="1801e-116">1</span><span class="sxs-lookup"><span data-stu-id="1801e-116">1</span></span>|<span data-ttu-id="1801e-117">Einem fehlerfreien Zustand.</span><span class="sxs-lookup"><span data-stu-id="1801e-117">Healthy state.</span></span>|
|<span data-ttu-id="1801e-118">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="1801e-118">unhealthy</span></span>|<span data-ttu-id="1801e-119">2</span><span class="sxs-lookup"><span data-stu-id="1801e-119">2</span></span>|<span data-ttu-id="1801e-120">Fehlerhaften Zustand.</span><span class="sxs-lookup"><span data-stu-id="1801e-120">Unhealthy state.</span></span>|





