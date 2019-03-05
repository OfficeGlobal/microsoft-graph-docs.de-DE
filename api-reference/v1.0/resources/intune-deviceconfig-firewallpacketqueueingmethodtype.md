---
title: firewallPacketQueueingMethodType-Enumerationstyp
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258926"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="59473-103">firewallPacketQueueingMethodType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="59473-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="59473-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="59473-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59473-105">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="59473-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="59473-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="59473-106">Members</span></span>
|<span data-ttu-id="59473-107">Element</span><span class="sxs-lookup"><span data-stu-id="59473-107">Member</span></span>|<span data-ttu-id="59473-108">Wert</span><span class="sxs-lookup"><span data-stu-id="59473-108">Value</span></span>|<span data-ttu-id="59473-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59473-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59473-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="59473-110">deviceDefault</span></span>|<span data-ttu-id="59473-111">0</span><span class="sxs-lookup"><span data-stu-id="59473-111">0</span></span>|<span data-ttu-id="59473-112">Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts</span><span class="sxs-lookup"><span data-stu-id="59473-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="59473-113">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="59473-113">disabled</span></span>|<span data-ttu-id="59473-114">1</span><span class="sxs-lookup"><span data-stu-id="59473-114">1</span></span>|<span data-ttu-id="59473-115">Deaktivieren von Paketwarteschlangen</span><span class="sxs-lookup"><span data-stu-id="59473-115">Disable packet queuing</span></span>|
|<span data-ttu-id="59473-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="59473-116">queueInbound</span></span>|<span data-ttu-id="59473-117">2</span><span class="sxs-lookup"><span data-stu-id="59473-117">2</span></span>|<span data-ttu-id="59473-118">Eingehende verschlüsselte Pakete in der Warteschlange</span><span class="sxs-lookup"><span data-stu-id="59473-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="59473-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="59473-119">queueOutbound</span></span>|<span data-ttu-id="59473-120">3</span><span class="sxs-lookup"><span data-stu-id="59473-120">3</span></span>|<span data-ttu-id="59473-121">Entschlüsselte ausgehende Pakete für die Weiterleitung in der Warteschlange</span><span class="sxs-lookup"><span data-stu-id="59473-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="59473-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="59473-122">queueBoth</span></span>|<span data-ttu-id="59473-123">4</span><span class="sxs-lookup"><span data-stu-id="59473-123">4</span></span>|<span data-ttu-id="59473-124">Warteschlange für ein-und ausgehende Pakete</span><span class="sxs-lookup"><span data-stu-id="59473-124">Queue both inbound and outbound packets</span></span>|



