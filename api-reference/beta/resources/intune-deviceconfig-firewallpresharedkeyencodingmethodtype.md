---
title: FirewallPreSharedKeyEncodingMethodType Enum-Typ
description: Mögliche Werte für firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513a6c545fedc73add4e710ed784ef223d1f8539
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976352"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="86d8e-103">FirewallPreSharedKeyEncodingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="86d8e-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="86d8e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="86d8e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86d8e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86d8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86d8e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="86d8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86d8e-107">Mögliche Werte für firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="86d8e-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="86d8e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="86d8e-108">Members</span></span>
|<span data-ttu-id="86d8e-109">Element</span><span class="sxs-lookup"><span data-stu-id="86d8e-109">Member</span></span>|<span data-ttu-id="86d8e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="86d8e-110">Value</span></span>|<span data-ttu-id="86d8e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86d8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86d8e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="86d8e-112">deviceDefault</span></span>|<span data-ttu-id="86d8e-113">0</span><span class="sxs-lookup"><span data-stu-id="86d8e-113">0</span></span>|<span data-ttu-id="86d8e-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="86d8e-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="86d8e-115">n/v</span><span class="sxs-lookup"><span data-stu-id="86d8e-115">none</span></span>|<span data-ttu-id="86d8e-116">1</span><span class="sxs-lookup"><span data-stu-id="86d8e-116">1</span></span>|<span data-ttu-id="86d8e-117">Vorinstallierter Schlüssel ist nicht codiert.</span><span class="sxs-lookup"><span data-stu-id="86d8e-117">Preshared key is not encoded.</span></span> <span data-ttu-id="86d8e-118">Stattdessen wird es in seinem Breitzeichen-Format gespeichert</span><span class="sxs-lookup"><span data-stu-id="86d8e-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="86d8e-119">utF8</span><span class="sxs-lookup"><span data-stu-id="86d8e-119">utF8</span></span>|<span data-ttu-id="86d8e-120">2</span><span class="sxs-lookup"><span data-stu-id="86d8e-120">2</span></span>|<span data-ttu-id="86d8e-121">Vorinstallierten Schlüssel mit UTF-8-Codierung</span><span class="sxs-lookup"><span data-stu-id="86d8e-121">Encode the preshared key using UTF-8</span></span>|





