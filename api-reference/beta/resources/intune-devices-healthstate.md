---
title: HealthState Enum-Typ
description: Gibt Integritätsstatus der Windows Management-app an.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b9104c0e39e086f7cf8f417f11054221b6f30e8d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422726"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="25443-103">HealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="25443-103">healthState enum type</span></span>

> <span data-ttu-id="25443-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="25443-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25443-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25443-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25443-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25443-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25443-107">Gibt Integritätsstatus der Windows Management-app an.</span><span class="sxs-lookup"><span data-stu-id="25443-107">Indicates health state of the Windows management app.</span></span>

## <a name="members"></a><span data-ttu-id="25443-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="25443-108">Members</span></span>
|<span data-ttu-id="25443-109">Member</span><span class="sxs-lookup"><span data-stu-id="25443-109">Member</span></span>|<span data-ttu-id="25443-110">Wert</span><span class="sxs-lookup"><span data-stu-id="25443-110">Value</span></span>|<span data-ttu-id="25443-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25443-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25443-112">unknown</span><span class="sxs-lookup"><span data-stu-id="25443-112">unknown</span></span>|<span data-ttu-id="25443-113">0</span><span class="sxs-lookup"><span data-stu-id="25443-113">0</span></span>|<span data-ttu-id="25443-114">Status ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="25443-114">Unknown state.</span></span>|
|<span data-ttu-id="25443-115">fehlerfrei</span><span class="sxs-lookup"><span data-stu-id="25443-115">healthy</span></span>|<span data-ttu-id="25443-116">1</span><span class="sxs-lookup"><span data-stu-id="25443-116">1</span></span>|<span data-ttu-id="25443-117">Einem fehlerfreien Zustand.</span><span class="sxs-lookup"><span data-stu-id="25443-117">Healthy state.</span></span>|
|<span data-ttu-id="25443-118">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="25443-118">unhealthy</span></span>|<span data-ttu-id="25443-119">2</span><span class="sxs-lookup"><span data-stu-id="25443-119">2</span></span>|<span data-ttu-id="25443-120">Fehlerhaften Zustand.</span><span class="sxs-lookup"><span data-stu-id="25443-120">Unhealthy state.</span></span>|




