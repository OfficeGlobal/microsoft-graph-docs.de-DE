---
title: Aktivierung von Steuerelementen Enum-Typ
description: 'Werte verwendet, um den Status eines Geräts angeben. '
ms.openlocfilehash: 5e72df98d33a7d3502dae4bc369781b69bc6aeb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061769"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="a8636-103">Aktivierung von Steuerelementen Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a8636-103">enablement enum type</span></span>

> <span data-ttu-id="a8636-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8636-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8636-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8636-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8636-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8636-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8636-107">Werte verwendet, um den Status eines Geräts angeben.</span><span class="sxs-lookup"><span data-stu-id="a8636-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="a8636-108">Beachten Sie, dass es ein Unterschied zwischen deaktiviert und nicht konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="a8636-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="a8636-109">Elemente</span><span class="sxs-lookup"><span data-stu-id="a8636-109">Members</span></span>
|<span data-ttu-id="a8636-110">Element</span><span class="sxs-lookup"><span data-stu-id="a8636-110">Member</span></span>|<span data-ttu-id="a8636-111">Wert</span><span class="sxs-lookup"><span data-stu-id="a8636-111">Value</span></span>|<span data-ttu-id="a8636-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8636-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8636-113">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="a8636-113">notConfigured</span></span>|<span data-ttu-id="a8636-114">0</span><span class="sxs-lookup"><span data-stu-id="a8636-114">0</span></span>|<span data-ttu-id="a8636-115">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="a8636-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="a8636-116">enabled</span><span class="sxs-lookup"><span data-stu-id="a8636-116">enabled</span></span>|<span data-ttu-id="a8636-117">1</span><span class="sxs-lookup"><span data-stu-id="a8636-117">1</span></span>|<span data-ttu-id="a8636-118">Aktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="a8636-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="a8636-119">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="a8636-119">disabled</span></span>|<span data-ttu-id="a8636-120">2</span><span class="sxs-lookup"><span data-stu-id="a8636-120">2</span></span>|<span data-ttu-id="a8636-121">Deaktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="a8636-121">Disables the setting on the device.</span></span>|
