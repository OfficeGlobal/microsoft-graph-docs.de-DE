---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2c494b6822a2a85cd4a3d295ac70b80efffcd10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885946"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="e8a79-103">ManagedAppDataEncryptionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e8a79-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="e8a79-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8a79-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8a79-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8a79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8a79-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e8a79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8a79-107">Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden</span><span class="sxs-lookup"><span data-stu-id="e8a79-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="e8a79-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e8a79-108">Members</span></span>
|<span data-ttu-id="e8a79-109">Element</span><span class="sxs-lookup"><span data-stu-id="e8a79-109">Member</span></span>|<span data-ttu-id="e8a79-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e8a79-110">Value</span></span>|<span data-ttu-id="e8a79-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8a79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8a79-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="e8a79-112">useDeviceSettings</span></span>|<span data-ttu-id="e8a79-113">0</span><span class="sxs-lookup"><span data-stu-id="e8a79-113">0</span></span>|<span data-ttu-id="e8a79-114">App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="e8a79-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="e8a79-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="e8a79-115">afterDeviceRestart</span></span>|<span data-ttu-id="e8a79-116">1</span><span class="sxs-lookup"><span data-stu-id="e8a79-116">1</span></span>|<span data-ttu-id="e8a79-117">App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="e8a79-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="e8a79-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="e8a79-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="e8a79-119">2</span><span class="sxs-lookup"><span data-stu-id="e8a79-119">2</span></span>|<span data-ttu-id="e8a79-120">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="e8a79-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="e8a79-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e8a79-121">whenDeviceLocked</span></span>|<span data-ttu-id="e8a79-122">3</span><span class="sxs-lookup"><span data-stu-id="e8a79-122">3</span></span>|<span data-ttu-id="e8a79-123">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="e8a79-123">App data associated with this policy is encrypted when the device is locked</span></span>|





