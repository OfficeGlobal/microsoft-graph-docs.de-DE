---
title: DeviceManagementExchangeConnectorType Enum-Typ
description: Der Typ des Exchange-Connectors.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07449df53aa65036ae55e63c514c1687fbbab86a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888515"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="5735b-103">DeviceManagementExchangeConnectorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5735b-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="5735b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5735b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5735b-105">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="5735b-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="5735b-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="5735b-106">Members</span></span>
|<span data-ttu-id="5735b-107">Element</span><span class="sxs-lookup"><span data-stu-id="5735b-107">Member</span></span>|<span data-ttu-id="5735b-108">Wert</span><span class="sxs-lookup"><span data-stu-id="5735b-108">Value</span></span>|<span data-ttu-id="5735b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5735b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5735b-110">"lokal"</span><span class="sxs-lookup"><span data-stu-id="5735b-110">onPremises</span></span>|<span data-ttu-id="5735b-111">0</span><span class="sxs-lookup"><span data-stu-id="5735b-111">0</span></span>|<span data-ttu-id="5735b-112">Stellt eine Verbindung zum lokalen Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="5735b-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="5735b-113">gehostet</span><span class="sxs-lookup"><span data-stu-id="5735b-113">hosted</span></span>|<span data-ttu-id="5735b-114">1</span><span class="sxs-lookup"><span data-stu-id="5735b-114">1</span></span>|<span data-ttu-id="5735b-115">Stellt eine Verbindung mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="5735b-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="5735b-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="5735b-116">serviceToService</span></span>|<span data-ttu-id="5735b-117">2</span><span class="sxs-lookup"><span data-stu-id="5735b-117">2</span></span>|<span data-ttu-id="5735b-118">Intune Service verbindet direkt mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="5735b-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="5735b-119">dedizierte</span><span class="sxs-lookup"><span data-stu-id="5735b-119">dedicated</span></span>|<span data-ttu-id="5735b-120">3</span><span class="sxs-lookup"><span data-stu-id="5735b-120">3</span></span>|<span data-ttu-id="5735b-121">Stellt eine Verbindung zu Office 365 dedizierte Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="5735b-121">Connects to O365 Dedicated Exchange environment.</span></span>|



