---
title: AndroidDeviceOwnerAppAutoUpdatePolicyType Enum-Typ
description: Android-Gerät Besitzer mögliche Werte für Status des Geräts app Auto Richtlinie aktualisiert werden.
ms.openlocfilehash: 0287a26b4974bc0b376341ca91791d1fa768a9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058149"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="cbbf9-103">AndroidDeviceOwnerAppAutoUpdatePolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cbbf9-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="cbbf9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbbf9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbbf9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbbf9-107">Android-Gerät Besitzer mögliche Werte für Status des Geräts app Auto Richtlinie aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="cbbf9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="cbbf9-108">Members</span></span>
|<span data-ttu-id="cbbf9-109">Element</span><span class="sxs-lookup"><span data-stu-id="cbbf9-109">Member</span></span>|<span data-ttu-id="cbbf9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="cbbf9-110">Value</span></span>|<span data-ttu-id="cbbf9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbbf9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbbf9-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="cbbf9-112">notConfigured</span></span>|<span data-ttu-id="cbbf9-113">0</span><span class="sxs-lookup"><span data-stu-id="cbbf9-113">0</span></span>|<span data-ttu-id="cbbf9-114">Nicht konfiguriert. Dieser Wert wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="cbbf9-115">UserChoice um</span><span class="sxs-lookup"><span data-stu-id="cbbf9-115">userChoice</span></span>|<span data-ttu-id="cbbf9-116">1</span><span class="sxs-lookup"><span data-stu-id="cbbf9-116">1</span></span>|<span data-ttu-id="cbbf9-117">Der Benutzer kann die automatische Updates steuern.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="cbbf9-118">nie</span><span class="sxs-lookup"><span data-stu-id="cbbf9-118">never</span></span>|<span data-ttu-id="cbbf9-119">2</span><span class="sxs-lookup"><span data-stu-id="cbbf9-119">2</span></span>|<span data-ttu-id="cbbf9-120">Apps werden nie mit automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="cbbf9-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="cbbf9-121">wiFiOnly</span></span>|<span data-ttu-id="cbbf9-122">3</span><span class="sxs-lookup"><span data-stu-id="cbbf9-122">3</span></span>|<span data-ttu-id="cbbf9-123">Apps werden automatisch aktualisiert über Wi-Fi nur.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="cbbf9-124">immer</span><span class="sxs-lookup"><span data-stu-id="cbbf9-124">always</span></span>|<span data-ttu-id="cbbf9-125">4</span><span class="sxs-lookup"><span data-stu-id="cbbf9-125">4</span></span>|<span data-ttu-id="cbbf9-126">Apps werden können Sie jederzeit automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="cbbf9-127">Daten können anfallen.</span><span class="sxs-lookup"><span data-stu-id="cbbf9-127">Data charges may apply.</span></span>|





