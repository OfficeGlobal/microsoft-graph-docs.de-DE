---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc40b93eebc17b1d1abcd9c317da1ffa538512a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425757"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="77276-103">FirewallPacketQueueingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="77276-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="77276-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="77276-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77276-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77276-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77276-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77276-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77276-107">Mögliche Werte für firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="77276-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="77276-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="77276-108">Members</span></span>
|<span data-ttu-id="77276-109">Member</span><span class="sxs-lookup"><span data-stu-id="77276-109">Member</span></span>|<span data-ttu-id="77276-110">Wert</span><span class="sxs-lookup"><span data-stu-id="77276-110">Value</span></span>|<span data-ttu-id="77276-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77276-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77276-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="77276-112">deviceDefault</span></span>|<span data-ttu-id="77276-113">0</span><span class="sxs-lookup"><span data-stu-id="77276-113">0</span></span>|<span data-ttu-id="77276-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="77276-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="77276-115">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="77276-115">disabled</span></span>|<span data-ttu-id="77276-116">1</span><span class="sxs-lookup"><span data-stu-id="77276-116">1</span></span>|<span data-ttu-id="77276-117">Paket Warteschlangen deaktivieren</span><span class="sxs-lookup"><span data-stu-id="77276-117">Disable packet queuing</span></span>|
|<span data-ttu-id="77276-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="77276-118">queueInbound</span></span>|<span data-ttu-id="77276-119">2</span><span class="sxs-lookup"><span data-stu-id="77276-119">2</span></span>|<span data-ttu-id="77276-120">Eingehende, verschlüsselte Pakete Warteschlange</span><span class="sxs-lookup"><span data-stu-id="77276-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="77276-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="77276-121">queueOutbound</span></span>|<span data-ttu-id="77276-122">3</span><span class="sxs-lookup"><span data-stu-id="77276-122">3</span></span>|<span data-ttu-id="77276-123">Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="77276-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="77276-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="77276-124">queueBoth</span></span>|<span data-ttu-id="77276-125">4</span><span class="sxs-lookup"><span data-stu-id="77276-125">4</span></span>|<span data-ttu-id="77276-126">Die Warteschlange eingehenden und ausgehenden Pakete</span><span class="sxs-lookup"><span data-stu-id="77276-126">Queue both inbound and outbound packets</span></span>|




