---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d9b4591ceff59becfa6f9fb17d490c56d59c9703
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833012"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="0e312-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0e312-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="0e312-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e312-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e312-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e312-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e312-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e312-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e312-107">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="0e312-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="0e312-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0e312-108">Members</span></span>
|<span data-ttu-id="0e312-109">Element</span><span class="sxs-lookup"><span data-stu-id="0e312-109">Member</span></span>|<span data-ttu-id="0e312-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0e312-110">Value</span></span>|<span data-ttu-id="0e312-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e312-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e312-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0e312-112">deviceDefault</span></span>|<span data-ttu-id="0e312-113">0</span><span class="sxs-lookup"><span data-stu-id="0e312-113">0</span></span>|<span data-ttu-id="0e312-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="0e312-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="0e312-115">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="0e312-115">disabled</span></span>|<span data-ttu-id="0e312-116">1</span><span class="sxs-lookup"><span data-stu-id="0e312-116">1</span></span>|<span data-ttu-id="0e312-117">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="0e312-117">Disable packet queuing</span></span>|
|<span data-ttu-id="0e312-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="0e312-118">queueInbound</span></span>|<span data-ttu-id="0e312-119">2</span><span class="sxs-lookup"><span data-stu-id="0e312-119">2</span></span>|<span data-ttu-id="0e312-120">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="0e312-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="0e312-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="0e312-121">queueOutbound</span></span>|<span data-ttu-id="0e312-122">3</span><span class="sxs-lookup"><span data-stu-id="0e312-122">3</span></span>|<span data-ttu-id="0e312-123">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="0e312-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="0e312-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="0e312-124">queueBoth</span></span>|<span data-ttu-id="0e312-125">4</span><span class="sxs-lookup"><span data-stu-id="0e312-125">4</span></span>|<span data-ttu-id="0e312-126">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="0e312-126">Queue both inbound and outbound packets</span></span>|





