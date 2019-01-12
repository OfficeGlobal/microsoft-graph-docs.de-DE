---
title: HealthState Enum-Typ
description: Gibt Integritätsstatus der Windows Management-app an.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b38dcefa57b467f688cc7b91ca2406250333ad1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922767"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="a7363-103">HealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a7363-103">healthState enum type</span></span>

> <span data-ttu-id="a7363-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7363-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7363-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7363-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7363-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a7363-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7363-107">Gibt Integritätsstatus der Windows Management-app an.</span><span class="sxs-lookup"><span data-stu-id="a7363-107">Indicates health state of the Windows management app.</span></span>
## <a name="members"></a><span data-ttu-id="a7363-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a7363-108">Members</span></span>
|<span data-ttu-id="a7363-109">Element</span><span class="sxs-lookup"><span data-stu-id="a7363-109">Member</span></span>|<span data-ttu-id="a7363-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a7363-110">Value</span></span>|<span data-ttu-id="a7363-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7363-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7363-112">unknown</span><span class="sxs-lookup"><span data-stu-id="a7363-112">unknown</span></span>|<span data-ttu-id="a7363-113">0</span><span class="sxs-lookup"><span data-stu-id="a7363-113">0</span></span>|<span data-ttu-id="a7363-114">Status ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="a7363-114">Unknown state.</span></span>|
|<span data-ttu-id="a7363-115">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="a7363-115">healthy</span></span>|<span data-ttu-id="a7363-116">1</span><span class="sxs-lookup"><span data-stu-id="a7363-116">1</span></span>|<span data-ttu-id="a7363-117">Einem fehlerfreien Zustand.</span><span class="sxs-lookup"><span data-stu-id="a7363-117">Healthy state.</span></span>|
|<span data-ttu-id="a7363-118">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="a7363-118">unhealthy</span></span>|<span data-ttu-id="a7363-119">2</span><span class="sxs-lookup"><span data-stu-id="a7363-119">2</span></span>|<span data-ttu-id="a7363-120">Fehlerhaften Zustand.</span><span class="sxs-lookup"><span data-stu-id="a7363-120">Unhealthy state.</span></span>|





