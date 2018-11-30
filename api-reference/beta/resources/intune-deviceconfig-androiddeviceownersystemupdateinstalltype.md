---
title: AndroidDeviceOwnerSystemUpdateInstallType Enum-Typ
description: Update-Systemtypen für Android-Gerät Besitzer.
ms.openlocfilehash: e9f23fd96ed0965b6693776858082e2df4925f37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062086"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="d5bc8-103">AndroidDeviceOwnerSystemUpdateInstallType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d5bc8-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="d5bc8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5bc8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5bc8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5bc8-107">Update-Systemtypen für Android-Gerät Besitzer.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="d5bc8-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d5bc8-108">Members</span></span>
|<span data-ttu-id="d5bc8-109">Element</span><span class="sxs-lookup"><span data-stu-id="d5bc8-109">Member</span></span>|<span data-ttu-id="d5bc8-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d5bc8-110">Value</span></span>|<span data-ttu-id="d5bc8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5bc8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5bc8-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d5bc8-112">deviceDefault</span></span>|<span data-ttu-id="d5bc8-113">0</span><span class="sxs-lookup"><span data-stu-id="d5bc8-113">0</span></span>|<span data-ttu-id="d5bc8-114">Gerät Standardverhalten in der Regel der Benutzer Systemupdates akzeptieren kann.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="d5bc8-115">Verschieben</span><span class="sxs-lookup"><span data-stu-id="d5bc8-115">postpone</span></span>|<span data-ttu-id="d5bc8-116">1</span><span class="sxs-lookup"><span data-stu-id="d5bc8-116">1</span></span>|<span data-ttu-id="d5bc8-117">Automatische Installation von Updates auf 30 Tage oben zu verschieben.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="d5bc8-118">Fenstermodus</span><span class="sxs-lookup"><span data-stu-id="d5bc8-118">windowed</span></span>|<span data-ttu-id="d5bc8-119">2</span><span class="sxs-lookup"><span data-stu-id="d5bc8-119">2</span></span>|<span data-ttu-id="d5bc8-120">Innerhalb eines tägliche Wartungsfensters automatisch installiert.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="d5bc8-121">Automatisch</span><span class="sxs-lookup"><span data-stu-id="d5bc8-121">automatic</span></span>|<span data-ttu-id="d5bc8-122">3</span><span class="sxs-lookup"><span data-stu-id="d5bc8-122">3</span></span>|<span data-ttu-id="d5bc8-123">Installieren Sie die Updates automatisch so bald wie möglich.</span><span class="sxs-lookup"><span data-stu-id="d5bc8-123">Automatically install updates as soon as possible.</span></span>|





