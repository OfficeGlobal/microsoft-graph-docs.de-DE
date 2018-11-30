---
title: DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ
description: Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058190"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="3d388-103">DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3d388-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="3d388-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3d388-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d388-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d388-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d388-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d388-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d388-107">Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="3d388-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="3d388-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3d388-108">Members</span></span>
|<span data-ttu-id="3d388-109">Element</span><span class="sxs-lookup"><span data-stu-id="3d388-109">Member</span></span>|<span data-ttu-id="3d388-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3d388-110">Value</span></span>|<span data-ttu-id="3d388-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d388-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d388-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="3d388-112">notConfigured</span></span>|<span data-ttu-id="3d388-113">0</span><span class="sxs-lookup"><span data-stu-id="3d388-113">0</span></span>|<span data-ttu-id="3d388-114">Schaltet Anmeldeinformationen Guard Remote Wenn zuvor ohne UEFI Sperre konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="3d388-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="3d388-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="3d388-115">enableWithUEFILock</span></span>|<span data-ttu-id="3d388-116">1</span><span class="sxs-lookup"><span data-stu-id="3d388-116">1</span></span>|<span data-ttu-id="3d388-117">Aktiviert die Anmeldeinformationen Guard mit UEFI sperren.</span><span class="sxs-lookup"><span data-stu-id="3d388-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="3d388-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="3d388-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="3d388-119">2</span><span class="sxs-lookup"><span data-stu-id="3d388-119">2</span></span>|<span data-ttu-id="3d388-120">Aktiviert die Anmeldeinformationen Guard ohne UEFI sperren.</span><span class="sxs-lookup"><span data-stu-id="3d388-120">Turns on Credential Guard without UEFI lock.</span></span>|





