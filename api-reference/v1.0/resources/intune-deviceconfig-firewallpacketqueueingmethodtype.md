---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1303287e521cf0b542047e8acaf122bc08a770a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823219"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="84d06-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="84d06-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="84d06-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84d06-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84d06-105">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="84d06-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="84d06-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="84d06-106">Members</span></span>
|<span data-ttu-id="84d06-107">Element</span><span class="sxs-lookup"><span data-stu-id="84d06-107">Member</span></span>|<span data-ttu-id="84d06-108">Wert</span><span class="sxs-lookup"><span data-stu-id="84d06-108">Value</span></span>|<span data-ttu-id="84d06-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84d06-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84d06-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="84d06-110">deviceDefault</span></span>|<span data-ttu-id="84d06-111">0</span><span class="sxs-lookup"><span data-stu-id="84d06-111">0</span></span>|<span data-ttu-id="84d06-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="84d06-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="84d06-113">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="84d06-113">disabled</span></span>|<span data-ttu-id="84d06-114">1</span><span class="sxs-lookup"><span data-stu-id="84d06-114">1</span></span>|<span data-ttu-id="84d06-115">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="84d06-115">Disable packet queuing</span></span>|
|<span data-ttu-id="84d06-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="84d06-116">queueInbound</span></span>|<span data-ttu-id="84d06-117">2</span><span class="sxs-lookup"><span data-stu-id="84d06-117">2</span></span>|<span data-ttu-id="84d06-118">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="84d06-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="84d06-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="84d06-119">queueOutbound</span></span>|<span data-ttu-id="84d06-120">3</span><span class="sxs-lookup"><span data-stu-id="84d06-120">3</span></span>|<span data-ttu-id="84d06-121">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="84d06-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="84d06-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="84d06-122">queueBoth</span></span>|<span data-ttu-id="84d06-123">4</span><span class="sxs-lookup"><span data-stu-id="84d06-123">4</span></span>|<span data-ttu-id="84d06-124">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="84d06-124">Queue both inbound and outbound packets</span></span>|



