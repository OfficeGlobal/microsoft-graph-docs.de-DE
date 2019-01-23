---
title: DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ
description: Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d8643744e1f5c36cf6c620ac85a6a99c9a77548
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398093"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="26e52-103">DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="26e52-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="26e52-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="26e52-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="26e52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26e52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26e52-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="26e52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e52-107">Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="26e52-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="26e52-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="26e52-108">Members</span></span>
|<span data-ttu-id="26e52-109">Member</span><span class="sxs-lookup"><span data-stu-id="26e52-109">Member</span></span>|<span data-ttu-id="26e52-110">Wert</span><span class="sxs-lookup"><span data-stu-id="26e52-110">Value</span></span>|<span data-ttu-id="26e52-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26e52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e52-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="26e52-112">notConfigured</span></span>|<span data-ttu-id="26e52-113">0</span><span class="sxs-lookup"><span data-stu-id="26e52-113">0</span></span>|<span data-ttu-id="26e52-114">Schaltet Anmeldeinformationen Guard Remote Wenn zuvor ohne UEFI Sperre konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="26e52-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="26e52-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="26e52-115">enableWithUEFILock</span></span>|<span data-ttu-id="26e52-116">1</span><span class="sxs-lookup"><span data-stu-id="26e52-116">1</span></span>|<span data-ttu-id="26e52-117">Aktiviert die Anmeldeinformationen Guard mit UEFI sperren.</span><span class="sxs-lookup"><span data-stu-id="26e52-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="26e52-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="26e52-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="26e52-119">2</span><span class="sxs-lookup"><span data-stu-id="26e52-119">2</span></span>|<span data-ttu-id="26e52-120">Aktiviert die Anmeldeinformationen Guard ohne UEFI sperren.</span><span class="sxs-lookup"><span data-stu-id="26e52-120">Turns on Credential Guard without UEFI lock.</span></span>|




