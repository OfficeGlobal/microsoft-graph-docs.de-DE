---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
ms.openlocfilehash: a642a3efc01f719ca72134f737fe2bdd2596d2b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064082"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="6b130-103">ManagedAppDataEncryptionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6b130-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="6b130-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b130-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b130-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b130-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b130-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6b130-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b130-107">Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden</span><span class="sxs-lookup"><span data-stu-id="6b130-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="6b130-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="6b130-108">Members</span></span>
|<span data-ttu-id="6b130-109">Element</span><span class="sxs-lookup"><span data-stu-id="6b130-109">Member</span></span>|<span data-ttu-id="6b130-110">Wert</span><span class="sxs-lookup"><span data-stu-id="6b130-110">Value</span></span>|<span data-ttu-id="6b130-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b130-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b130-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="6b130-112">useDeviceSettings</span></span>|<span data-ttu-id="6b130-113">0</span><span class="sxs-lookup"><span data-stu-id="6b130-113">0</span></span>|<span data-ttu-id="6b130-114">App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="6b130-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="6b130-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="6b130-115">afterDeviceRestart</span></span>|<span data-ttu-id="6b130-116">1</span><span class="sxs-lookup"><span data-stu-id="6b130-116">1</span></span>|<span data-ttu-id="6b130-117">App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="6b130-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="6b130-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="6b130-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="6b130-119">2</span><span class="sxs-lookup"><span data-stu-id="6b130-119">2</span></span>|<span data-ttu-id="6b130-120">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="6b130-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="6b130-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6b130-121">whenDeviceLocked</span></span>|<span data-ttu-id="6b130-122">3</span><span class="sxs-lookup"><span data-stu-id="6b130-122">3</span></span>|<span data-ttu-id="6b130-123">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="6b130-123">App data associated with this policy is encrypted when the device is locked</span></span>|





