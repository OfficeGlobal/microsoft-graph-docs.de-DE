---
title: firewallPreSharedKeyEncodingMethodType-Enumerationstyp
description: Mögliche Werte für firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62144ef2974da5a3d975c759bb8d2bd2be6032
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259549"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="fdc70-103">firewallPreSharedKeyEncodingMethodType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="fdc70-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="fdc70-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fdc70-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc70-105">Mögliche Werte für firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="fdc70-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="fdc70-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="fdc70-106">Members</span></span>
|<span data-ttu-id="fdc70-107">Element</span><span class="sxs-lookup"><span data-stu-id="fdc70-107">Member</span></span>|<span data-ttu-id="fdc70-108">Wert</span><span class="sxs-lookup"><span data-stu-id="fdc70-108">Value</span></span>|<span data-ttu-id="fdc70-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdc70-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc70-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fdc70-110">deviceDefault</span></span>|<span data-ttu-id="fdc70-111">0</span><span class="sxs-lookup"><span data-stu-id="fdc70-111">0</span></span>|<span data-ttu-id="fdc70-112">Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts</span><span class="sxs-lookup"><span data-stu-id="fdc70-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="fdc70-113">Keine</span><span class="sxs-lookup"><span data-stu-id="fdc70-113">none</span></span>|<span data-ttu-id="fdc70-114">1</span><span class="sxs-lookup"><span data-stu-id="fdc70-114">1</span></span>|<span data-ttu-id="fdc70-115">Der vorinstallierte Schlüssel ist nicht codiert.</span><span class="sxs-lookup"><span data-stu-id="fdc70-115">Preshared key is not encoded.</span></span> <span data-ttu-id="fdc70-116">Stattdessen wird es im Breitzeichen Format beibehalten.</span><span class="sxs-lookup"><span data-stu-id="fdc70-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="fdc70-117">utF8</span><span class="sxs-lookup"><span data-stu-id="fdc70-117">utF8</span></span>|<span data-ttu-id="fdc70-118">2</span><span class="sxs-lookup"><span data-stu-id="fdc70-118">2</span></span>|<span data-ttu-id="fdc70-119">Codieren des vorinstallierten Schlüssels mithilfe von UTF-8</span><span class="sxs-lookup"><span data-stu-id="fdc70-119">Encode the preshared key using UTF-8</span></span>|



