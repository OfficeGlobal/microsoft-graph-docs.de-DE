---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
ms.openlocfilehash: 9f3d63b7e58b6f9c5ba369c3ceb12d06704c4725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304557"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="1203b-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1203b-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="1203b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1203b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1203b-105">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1203b-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="1203b-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="1203b-106">Members</span></span>
|<span data-ttu-id="1203b-107">Member</span><span class="sxs-lookup"><span data-stu-id="1203b-107">Member</span></span>|<span data-ttu-id="1203b-108">Wert</span><span class="sxs-lookup"><span data-stu-id="1203b-108">Value</span></span>|<span data-ttu-id="1203b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1203b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1203b-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1203b-110">deviceDefault</span></span>|<span data-ttu-id="1203b-111">0</span><span class="sxs-lookup"><span data-stu-id="1203b-111">0</span></span>|<span data-ttu-id="1203b-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="1203b-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1203b-113">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="1203b-113">disabled</span></span>|<span data-ttu-id="1203b-114">1</span><span class="sxs-lookup"><span data-stu-id="1203b-114">1</span></span>|<span data-ttu-id="1203b-115">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="1203b-115">Disable packet queuing</span></span>|
|<span data-ttu-id="1203b-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="1203b-116">queueInbound</span></span>|<span data-ttu-id="1203b-117">2</span><span class="sxs-lookup"><span data-stu-id="1203b-117">2</span></span>|<span data-ttu-id="1203b-118">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="1203b-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="1203b-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="1203b-119">queueOutbound</span></span>|<span data-ttu-id="1203b-120">3</span><span class="sxs-lookup"><span data-stu-id="1203b-120">3</span></span>|<span data-ttu-id="1203b-121">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="1203b-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="1203b-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="1203b-122">queueBoth</span></span>|<span data-ttu-id="1203b-123">4</span><span class="sxs-lookup"><span data-stu-id="1203b-123">4</span></span>|<span data-ttu-id="1203b-124">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="1203b-124">Queue both inbound and outbound packets</span></span>|



