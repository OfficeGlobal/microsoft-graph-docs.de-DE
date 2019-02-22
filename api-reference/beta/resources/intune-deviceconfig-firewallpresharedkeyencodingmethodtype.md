---
title: firewallPreSharedKeyEncodingMethodType-Enumerationstyp
description: Mögliche Werte für firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e3a74122f0b0a9fe1a6dfab40593123ec8709c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160816"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="bed96-103">firewallPreSharedKeyEncodingMethodType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="bed96-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="bed96-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bed96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bed96-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bed96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed96-106">Mögliche Werte für firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="bed96-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="bed96-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="bed96-107">Members</span></span>
|<span data-ttu-id="bed96-108">Element</span><span class="sxs-lookup"><span data-stu-id="bed96-108">Member</span></span>|<span data-ttu-id="bed96-109">Wert</span><span class="sxs-lookup"><span data-stu-id="bed96-109">Value</span></span>|<span data-ttu-id="bed96-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bed96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed96-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="bed96-111">deviceDefault</span></span>|<span data-ttu-id="bed96-112">0</span><span class="sxs-lookup"><span data-stu-id="bed96-112">0</span></span>|<span data-ttu-id="bed96-113">Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts</span><span class="sxs-lookup"><span data-stu-id="bed96-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="bed96-114">Keine</span><span class="sxs-lookup"><span data-stu-id="bed96-114">none</span></span>|<span data-ttu-id="bed96-115">1</span><span class="sxs-lookup"><span data-stu-id="bed96-115">1</span></span>|<span data-ttu-id="bed96-116">Der vorinstallierte Schlüssel ist nicht codiert.</span><span class="sxs-lookup"><span data-stu-id="bed96-116">Preshared key is not encoded.</span></span> <span data-ttu-id="bed96-117">Stattdessen wird es im Breitzeichen Format beibehalten.</span><span class="sxs-lookup"><span data-stu-id="bed96-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="bed96-118">utF8</span><span class="sxs-lookup"><span data-stu-id="bed96-118">utF8</span></span>|<span data-ttu-id="bed96-119">2</span><span class="sxs-lookup"><span data-stu-id="bed96-119">2</span></span>|<span data-ttu-id="bed96-120">Codieren des vorinstallierten Schlüssels mithilfe von UTF-8</span><span class="sxs-lookup"><span data-stu-id="bed96-120">Encode the preshared key using UTF-8</span></span>|




