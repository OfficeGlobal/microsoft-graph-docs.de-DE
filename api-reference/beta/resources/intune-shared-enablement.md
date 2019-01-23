---
title: Aktivierung von Steuerelementen Enum-Typ
description: Beschreibt die Aktivierung von Steuerelementen Enumeration die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399563"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="5af36-103">Aktivierung von Steuerelementen Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5af36-103">enablement enum type</span></span>

> <span data-ttu-id="5af36-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5af36-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5af36-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5af36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5af36-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5af36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5af36-107">Werte verwendet, um den Status eines Geräts angeben.</span><span class="sxs-lookup"><span data-stu-id="5af36-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="5af36-108">Beachten Sie, dass es ein Unterschied zwischen deaktiviert und nicht konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="5af36-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="5af36-109">Elemente</span><span class="sxs-lookup"><span data-stu-id="5af36-109">Members</span></span>
|<span data-ttu-id="5af36-110">Member</span><span class="sxs-lookup"><span data-stu-id="5af36-110">Member</span></span>|<span data-ttu-id="5af36-111">Wert</span><span class="sxs-lookup"><span data-stu-id="5af36-111">Value</span></span>|<span data-ttu-id="5af36-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5af36-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af36-113">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="5af36-113">notConfigured</span></span>|<span data-ttu-id="5af36-114">0</span><span class="sxs-lookup"><span data-stu-id="5af36-114">0</span></span>|<span data-ttu-id="5af36-115">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="5af36-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="5af36-116">enabled</span><span class="sxs-lookup"><span data-stu-id="5af36-116">enabled</span></span>|<span data-ttu-id="5af36-117">1</span><span class="sxs-lookup"><span data-stu-id="5af36-117">1</span></span>|<span data-ttu-id="5af36-118">Aktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="5af36-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="5af36-119">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="5af36-119">disabled</span></span>|<span data-ttu-id="5af36-120">2</span><span class="sxs-lookup"><span data-stu-id="5af36-120">2</span></span>|<span data-ttu-id="5af36-121">Deaktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="5af36-121">Disables the setting on the device.</span></span>|
