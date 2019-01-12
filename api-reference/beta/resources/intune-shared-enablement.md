---
title: Aktivierung von Steuerelementen Enum-Typ
description: 'Werte verwendet, um den Status eines Geräts angeben. '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 539d57111003f348147a6be3952d969ab4206b5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911959"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="fe92b-103">Aktivierung von Steuerelementen Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fe92b-103">enablement enum type</span></span>

> <span data-ttu-id="fe92b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe92b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe92b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe92b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe92b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fe92b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe92b-107">Werte verwendet, um den Status eines Geräts angeben.</span><span class="sxs-lookup"><span data-stu-id="fe92b-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="fe92b-108">Beachten Sie, dass es ein Unterschied zwischen deaktiviert und nicht konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="fe92b-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="fe92b-109">Elemente</span><span class="sxs-lookup"><span data-stu-id="fe92b-109">Members</span></span>
|<span data-ttu-id="fe92b-110">Element</span><span class="sxs-lookup"><span data-stu-id="fe92b-110">Member</span></span>|<span data-ttu-id="fe92b-111">Wert</span><span class="sxs-lookup"><span data-stu-id="fe92b-111">Value</span></span>|<span data-ttu-id="fe92b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe92b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe92b-113">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="fe92b-113">notConfigured</span></span>|<span data-ttu-id="fe92b-114">0</span><span class="sxs-lookup"><span data-stu-id="fe92b-114">0</span></span>|<span data-ttu-id="fe92b-115">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="fe92b-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="fe92b-116">enabled</span><span class="sxs-lookup"><span data-stu-id="fe92b-116">enabled</span></span>|<span data-ttu-id="fe92b-117">1</span><span class="sxs-lookup"><span data-stu-id="fe92b-117">1</span></span>|<span data-ttu-id="fe92b-118">Aktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="fe92b-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="fe92b-119">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="fe92b-119">disabled</span></span>|<span data-ttu-id="fe92b-120">2</span><span class="sxs-lookup"><span data-stu-id="fe92b-120">2</span></span>|<span data-ttu-id="fe92b-121">Deaktiviert die Einstellung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="fe92b-121">Disables the setting on the device.</span></span>|
