---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3700df6d2eaf0dd0d2dde8a3f4a90be2e3684951
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940099"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="e5e35-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e5e35-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="e5e35-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e5e35-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5e35-105">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="e5e35-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="e5e35-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="e5e35-106">Members</span></span>
|<span data-ttu-id="e5e35-107">Element</span><span class="sxs-lookup"><span data-stu-id="e5e35-107">Member</span></span>|<span data-ttu-id="e5e35-108">Wert</span><span class="sxs-lookup"><span data-stu-id="e5e35-108">Value</span></span>|<span data-ttu-id="e5e35-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5e35-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e35-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e5e35-110">deviceDefault</span></span>|<span data-ttu-id="e5e35-111">0</span><span class="sxs-lookup"><span data-stu-id="e5e35-111">0</span></span>|<span data-ttu-id="e5e35-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="e5e35-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="e5e35-113">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="e5e35-113">disabled</span></span>|<span data-ttu-id="e5e35-114">1</span><span class="sxs-lookup"><span data-stu-id="e5e35-114">1</span></span>|<span data-ttu-id="e5e35-115">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="e5e35-115">Disable packet queuing</span></span>|
|<span data-ttu-id="e5e35-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="e5e35-116">queueInbound</span></span>|<span data-ttu-id="e5e35-117">2</span><span class="sxs-lookup"><span data-stu-id="e5e35-117">2</span></span>|<span data-ttu-id="e5e35-118">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="e5e35-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="e5e35-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="e5e35-119">queueOutbound</span></span>|<span data-ttu-id="e5e35-120">3</span><span class="sxs-lookup"><span data-stu-id="e5e35-120">3</span></span>|<span data-ttu-id="e5e35-121">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="e5e35-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="e5e35-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="e5e35-122">queueBoth</span></span>|<span data-ttu-id="e5e35-123">4</span><span class="sxs-lookup"><span data-stu-id="e5e35-123">4</span></span>|<span data-ttu-id="e5e35-124">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="e5e35-124">Queue both inbound and outbound packets</span></span>|



