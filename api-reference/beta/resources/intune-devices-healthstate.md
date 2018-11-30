---
title: HealthState Enum-Typ
description: Gibt Integritätsstatus der Windows Management-app an.
ms.openlocfilehash: d52b894983795c9cb46d92dce6985e4aab3dd94d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065941"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="72bb9-103">HealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="72bb9-103">healthState enum type</span></span>

> <span data-ttu-id="72bb9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="72bb9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72bb9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72bb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72bb9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="72bb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72bb9-107">Gibt Integritätsstatus der Windows Management-app an.</span><span class="sxs-lookup"><span data-stu-id="72bb9-107">Indicates health state of the Windows management app.</span></span>
## <a name="members"></a><span data-ttu-id="72bb9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="72bb9-108">Members</span></span>
|<span data-ttu-id="72bb9-109">Element</span><span class="sxs-lookup"><span data-stu-id="72bb9-109">Member</span></span>|<span data-ttu-id="72bb9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="72bb9-110">Value</span></span>|<span data-ttu-id="72bb9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72bb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72bb9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="72bb9-112">unknown</span></span>|<span data-ttu-id="72bb9-113">0</span><span class="sxs-lookup"><span data-stu-id="72bb9-113">0</span></span>|<span data-ttu-id="72bb9-114">Status ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="72bb9-114">Unknown state.</span></span>|
|<span data-ttu-id="72bb9-115">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="72bb9-115">healthy</span></span>|<span data-ttu-id="72bb9-116">1</span><span class="sxs-lookup"><span data-stu-id="72bb9-116">1</span></span>|<span data-ttu-id="72bb9-117">Einem fehlerfreien Zustand.</span><span class="sxs-lookup"><span data-stu-id="72bb9-117">Healthy state.</span></span>|
|<span data-ttu-id="72bb9-118">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="72bb9-118">unhealthy</span></span>|<span data-ttu-id="72bb9-119">2</span><span class="sxs-lookup"><span data-stu-id="72bb9-119">2</span></span>|<span data-ttu-id="72bb9-120">Fehlerhaften Zustand.</span><span class="sxs-lookup"><span data-stu-id="72bb9-120">Unhealthy state.</span></span>|





