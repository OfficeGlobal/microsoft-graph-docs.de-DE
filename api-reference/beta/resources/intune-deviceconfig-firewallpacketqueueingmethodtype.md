---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9538db02afc108573338556c8899495ca9c1f26c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957795"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="b10a6-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b10a6-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="b10a6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b10a6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b10a6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b10a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b10a6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b10a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b10a6-107">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b10a6-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="b10a6-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b10a6-108">Members</span></span>
|<span data-ttu-id="b10a6-109">Element</span><span class="sxs-lookup"><span data-stu-id="b10a6-109">Member</span></span>|<span data-ttu-id="b10a6-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b10a6-110">Value</span></span>|<span data-ttu-id="b10a6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b10a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b10a6-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b10a6-112">deviceDefault</span></span>|<span data-ttu-id="b10a6-113">0</span><span class="sxs-lookup"><span data-stu-id="b10a6-113">0</span></span>|<span data-ttu-id="b10a6-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="b10a6-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b10a6-115">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="b10a6-115">disabled</span></span>|<span data-ttu-id="b10a6-116">1</span><span class="sxs-lookup"><span data-stu-id="b10a6-116">1</span></span>|<span data-ttu-id="b10a6-117">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="b10a6-117">Disable packet queuing</span></span>|
|<span data-ttu-id="b10a6-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="b10a6-118">queueInbound</span></span>|<span data-ttu-id="b10a6-119">2</span><span class="sxs-lookup"><span data-stu-id="b10a6-119">2</span></span>|<span data-ttu-id="b10a6-120">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="b10a6-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="b10a6-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="b10a6-121">queueOutbound</span></span>|<span data-ttu-id="b10a6-122">3</span><span class="sxs-lookup"><span data-stu-id="b10a6-122">3</span></span>|<span data-ttu-id="b10a6-123">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="b10a6-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="b10a6-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="b10a6-124">queueBoth</span></span>|<span data-ttu-id="b10a6-125">4</span><span class="sxs-lookup"><span data-stu-id="b10a6-125">4</span></span>|<span data-ttu-id="b10a6-126">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="b10a6-126">Queue both inbound and outbound packets</span></span>|





