---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
ms.openlocfilehash: f55b68780d3bec97fa48a32c7abd8e1cfb269755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063272"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="f9d56-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f9d56-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="f9d56-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9d56-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9d56-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9d56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9d56-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f9d56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9d56-107">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="f9d56-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="f9d56-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f9d56-108">Members</span></span>
|<span data-ttu-id="f9d56-109">Element</span><span class="sxs-lookup"><span data-stu-id="f9d56-109">Member</span></span>|<span data-ttu-id="f9d56-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f9d56-110">Value</span></span>|<span data-ttu-id="f9d56-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9d56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9d56-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f9d56-112">deviceDefault</span></span>|<span data-ttu-id="f9d56-113">0</span><span class="sxs-lookup"><span data-stu-id="f9d56-113">0</span></span>|<span data-ttu-id="f9d56-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="f9d56-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f9d56-115">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="f9d56-115">disabled</span></span>|<span data-ttu-id="f9d56-116">1</span><span class="sxs-lookup"><span data-stu-id="f9d56-116">1</span></span>|<span data-ttu-id="f9d56-117">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="f9d56-117">Disable packet queuing</span></span>|
|<span data-ttu-id="f9d56-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="f9d56-118">queueInbound</span></span>|<span data-ttu-id="f9d56-119">2</span><span class="sxs-lookup"><span data-stu-id="f9d56-119">2</span></span>|<span data-ttu-id="f9d56-120">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="f9d56-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="f9d56-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="f9d56-121">queueOutbound</span></span>|<span data-ttu-id="f9d56-122">3</span><span class="sxs-lookup"><span data-stu-id="f9d56-122">3</span></span>|<span data-ttu-id="f9d56-123">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="f9d56-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="f9d56-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="f9d56-124">queueBoth</span></span>|<span data-ttu-id="f9d56-125">4</span><span class="sxs-lookup"><span data-stu-id="f9d56-125">4</span></span>|<span data-ttu-id="f9d56-126">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="f9d56-126">Queue both inbound and outbound packets</span></span>|





