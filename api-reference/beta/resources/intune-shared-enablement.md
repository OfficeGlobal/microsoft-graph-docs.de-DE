---
title: Aktivierung von Steuerelementen Enum-Typ
description: 'Werte verwendet, um den Status eines Geräts angeben. '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c77da7026640e9ad0a6f6f08f077d509cb411f22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888256"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="ebfee-103">Aktivierung von Steuerelementen Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ebfee-103">enablement enum type</span></span>

> <span data-ttu-id="ebfee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ebfee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebfee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebfee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebfee-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ebfee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebfee-107">Werte verwendet, um den Status eines Geräts angeben.</span><span class="sxs-lookup"><span data-stu-id="ebfee-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="ebfee-108">Beachten Sie, dass es ein Unterschied zwischen deaktiviert und nicht konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="ebfee-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="ebfee-109">Elemente</span><span class="sxs-lookup"><span data-stu-id="ebfee-109">Members</span></span>
|<span data-ttu-id="ebfee-110">Element</span><span class="sxs-lookup"><span data-stu-id="ebfee-110">Member</span></span>|<span data-ttu-id="ebfee-111">Wert</span><span class="sxs-lookup"><span data-stu-id="ebfee-111">Value</span></span>|<span data-ttu-id="ebfee-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebfee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfee-113">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="ebfee-113">notConfigured</span></span>|<span data-ttu-id="ebfee-114">0</span><span class="sxs-lookup"><span data-stu-id="ebfee-114">0</span></span>|<span data-ttu-id="ebfee-115">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="ebfee-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="ebfee-116">enabled</span><span class="sxs-lookup"><span data-stu-id="ebfee-116">enabled</span></span>|<span data-ttu-id="ebfee-117">1</span><span class="sxs-lookup"><span data-stu-id="ebfee-117">1</span></span>|<span data-ttu-id="ebfee-118">Aktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="ebfee-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="ebfee-119">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="ebfee-119">disabled</span></span>|<span data-ttu-id="ebfee-120">2</span><span class="sxs-lookup"><span data-stu-id="ebfee-120">2</span></span>|<span data-ttu-id="ebfee-121">Deaktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="ebfee-121">Disables the setting on the device.</span></span>|
