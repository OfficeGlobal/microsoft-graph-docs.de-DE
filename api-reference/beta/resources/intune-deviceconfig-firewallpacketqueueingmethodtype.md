---
title: firewallPacketQueueingMethodType-Enumerationstyp
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1b8543df5fa2a50cfdfa56c7cb2d96199ba44e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172205"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="62899-103">firewallPacketQueueingMethodType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="62899-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="62899-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62899-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62899-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="62899-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62899-106">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="62899-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="62899-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="62899-107">Members</span></span>
|<span data-ttu-id="62899-108">Element</span><span class="sxs-lookup"><span data-stu-id="62899-108">Member</span></span>|<span data-ttu-id="62899-109">Wert</span><span class="sxs-lookup"><span data-stu-id="62899-109">Value</span></span>|<span data-ttu-id="62899-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62899-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62899-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="62899-111">deviceDefault</span></span>|<span data-ttu-id="62899-112">0</span><span class="sxs-lookup"><span data-stu-id="62899-112">0</span></span>|<span data-ttu-id="62899-113">Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts</span><span class="sxs-lookup"><span data-stu-id="62899-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="62899-114">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="62899-114">disabled</span></span>|<span data-ttu-id="62899-115">1</span><span class="sxs-lookup"><span data-stu-id="62899-115">1</span></span>|<span data-ttu-id="62899-116">Deaktivieren von Paketwarteschlangen</span><span class="sxs-lookup"><span data-stu-id="62899-116">Disable packet queuing</span></span>|
|<span data-ttu-id="62899-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="62899-117">queueInbound</span></span>|<span data-ttu-id="62899-118">2</span><span class="sxs-lookup"><span data-stu-id="62899-118">2</span></span>|<span data-ttu-id="62899-119">Eingehende verschlüsselte Pakete in der Warteschlange</span><span class="sxs-lookup"><span data-stu-id="62899-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="62899-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="62899-120">queueOutbound</span></span>|<span data-ttu-id="62899-121">3</span><span class="sxs-lookup"><span data-stu-id="62899-121">3</span></span>|<span data-ttu-id="62899-122">Entschlüsselte ausgehende Pakete für die Weiterleitung in der Warteschlange</span><span class="sxs-lookup"><span data-stu-id="62899-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="62899-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="62899-123">queueBoth</span></span>|<span data-ttu-id="62899-124">4</span><span class="sxs-lookup"><span data-stu-id="62899-124">4</span></span>|<span data-ttu-id="62899-125">Warteschlange für ein-und ausgehende Pakete</span><span class="sxs-lookup"><span data-stu-id="62899-125">Queue both inbound and outbound packets</span></span>|




