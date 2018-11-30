---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
ms.openlocfilehash: 70643e300f1a6cc151edeae849e5ae7c5f977750
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018220"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="711b6-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="711b6-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="711b6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="711b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="711b6-105">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="711b6-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="711b6-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="711b6-106">Members</span></span>
|<span data-ttu-id="711b6-107">Element</span><span class="sxs-lookup"><span data-stu-id="711b6-107">Member</span></span>|<span data-ttu-id="711b6-108">Wert</span><span class="sxs-lookup"><span data-stu-id="711b6-108">Value</span></span>|<span data-ttu-id="711b6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="711b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="711b6-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="711b6-110">deviceDefault</span></span>|<span data-ttu-id="711b6-111">0</span><span class="sxs-lookup"><span data-stu-id="711b6-111">0</span></span>|<span data-ttu-id="711b6-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="711b6-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="711b6-113">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="711b6-113">disabled</span></span>|<span data-ttu-id="711b6-114">1</span><span class="sxs-lookup"><span data-stu-id="711b6-114">1</span></span>|<span data-ttu-id="711b6-115">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="711b6-115">Disable packet queuing</span></span>|
|<span data-ttu-id="711b6-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="711b6-116">queueInbound</span></span>|<span data-ttu-id="711b6-117">2</span><span class="sxs-lookup"><span data-stu-id="711b6-117">2</span></span>|<span data-ttu-id="711b6-118">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="711b6-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="711b6-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="711b6-119">queueOutbound</span></span>|<span data-ttu-id="711b6-120">3</span><span class="sxs-lookup"><span data-stu-id="711b6-120">3</span></span>|<span data-ttu-id="711b6-121">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="711b6-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="711b6-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="711b6-122">queueBoth</span></span>|<span data-ttu-id="711b6-123">4</span><span class="sxs-lookup"><span data-stu-id="711b6-123">4</span></span>|<span data-ttu-id="711b6-124">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="711b6-124">Queue both inbound and outbound packets</span></span>|



