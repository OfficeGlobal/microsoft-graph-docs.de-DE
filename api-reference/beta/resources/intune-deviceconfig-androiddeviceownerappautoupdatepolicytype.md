---
title: androidDeviceOwnerAppAutoUpdatePolicyType-Enumerationstyp
description: Android-Gerätebesitzer mögliche Werte für Status der APP-AutoUpdate-Richtlinie des Geräts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6242bc9470661d75b3174198761cfcab8284381d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159255"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="ae5b1-103">androidDeviceOwnerAppAutoUpdatePolicyType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="ae5b1-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="ae5b1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae5b1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae5b1-106">Android-Gerätebesitzer mögliche Werte für Status der APP-AutoUpdate-Richtlinie des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="ae5b1-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="ae5b1-107">Members</span></span>
|<span data-ttu-id="ae5b1-108">Element</span><span class="sxs-lookup"><span data-stu-id="ae5b1-108">Member</span></span>|<span data-ttu-id="ae5b1-109">Wert</span><span class="sxs-lookup"><span data-stu-id="ae5b1-109">Value</span></span>|<span data-ttu-id="ae5b1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae5b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae5b1-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ae5b1-111">notConfigured</span></span>|<span data-ttu-id="ae5b1-112">0</span><span class="sxs-lookup"><span data-stu-id="ae5b1-112">0</span></span>|<span data-ttu-id="ae5b1-113">Nicht konfiguriert; Dieser Wert wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="ae5b1-114">userChoice</span><span class="sxs-lookup"><span data-stu-id="ae5b1-114">userChoice</span></span>|<span data-ttu-id="ae5b1-115">1</span><span class="sxs-lookup"><span data-stu-id="ae5b1-115">1</span></span>|<span data-ttu-id="ae5b1-116">Der Benutzer kann AutoUpdates steuern.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="ae5b1-117">nie</span><span class="sxs-lookup"><span data-stu-id="ae5b1-117">never</span></span>|<span data-ttu-id="ae5b1-118">2</span><span class="sxs-lookup"><span data-stu-id="ae5b1-118">2</span></span>|<span data-ttu-id="ae5b1-119">Apps werden nie automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="ae5b1-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="ae5b1-120">wiFiOnly</span></span>|<span data-ttu-id="ae5b1-121">3</span><span class="sxs-lookup"><span data-stu-id="ae5b1-121">3</span></span>|<span data-ttu-id="ae5b1-122">Apps werden nur über WLAN automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="ae5b1-123">immer</span><span class="sxs-lookup"><span data-stu-id="ae5b1-123">always</span></span>|<span data-ttu-id="ae5b1-124">4</span><span class="sxs-lookup"><span data-stu-id="ae5b1-124">4</span></span>|<span data-ttu-id="ae5b1-125">Apps werden jederzeit automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="ae5b1-126">Es können Daten erhoben werden.</span><span class="sxs-lookup"><span data-stu-id="ae5b1-126">Data charges may apply.</span></span>|




