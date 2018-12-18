---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
author: tfitzmac
ms.openlocfilehash: 3cbb733eb578ca839e32851d8a6d217f69d6799d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330324"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="df2e1-103">ManagedAppDataEncryptionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="df2e1-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="df2e1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df2e1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df2e1-105">Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden</span><span class="sxs-lookup"><span data-stu-id="df2e1-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="df2e1-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="df2e1-106">Members</span></span>
|<span data-ttu-id="df2e1-107">Member</span><span class="sxs-lookup"><span data-stu-id="df2e1-107">Member</span></span>|<span data-ttu-id="df2e1-108">Wert</span><span class="sxs-lookup"><span data-stu-id="df2e1-108">Value</span></span>|<span data-ttu-id="df2e1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df2e1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df2e1-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="df2e1-110">useDeviceSettings</span></span>|<span data-ttu-id="df2e1-111">0</span><span class="sxs-lookup"><span data-stu-id="df2e1-111">0</span></span>|<span data-ttu-id="df2e1-112">App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="df2e1-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="df2e1-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="df2e1-113">afterDeviceRestart</span></span>|<span data-ttu-id="df2e1-114">1</span><span class="sxs-lookup"><span data-stu-id="df2e1-114">1</span></span>|<span data-ttu-id="df2e1-115">App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="df2e1-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="df2e1-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="df2e1-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="df2e1-117">2</span><span class="sxs-lookup"><span data-stu-id="df2e1-117">2</span></span>|<span data-ttu-id="df2e1-118">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="df2e1-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="df2e1-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="df2e1-119">whenDeviceLocked</span></span>|<span data-ttu-id="df2e1-120">3</span><span class="sxs-lookup"><span data-stu-id="df2e1-120">3</span></span>|<span data-ttu-id="df2e1-121">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="df2e1-121">App data associated with this policy is encrypted when the device is locked</span></span>|



