---
title: DeviceManagementExchangeConnectorType Enum-Typ
description: Der Typ des Exchange-Connectors.
author: tfitzmac
ms.openlocfilehash: 31459d4053e2ba1ef22a516995796baef2407dbf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301729"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="23f1b-103">DeviceManagementExchangeConnectorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="23f1b-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="23f1b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23f1b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23f1b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23f1b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23f1b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23f1b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23f1b-107">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="23f1b-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="23f1b-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="23f1b-108">Members</span></span>
|<span data-ttu-id="23f1b-109">Member</span><span class="sxs-lookup"><span data-stu-id="23f1b-109">Member</span></span>|<span data-ttu-id="23f1b-110">Wert</span><span class="sxs-lookup"><span data-stu-id="23f1b-110">Value</span></span>|<span data-ttu-id="23f1b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23f1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f1b-112">"lokal"</span><span class="sxs-lookup"><span data-stu-id="23f1b-112">onPremises</span></span>|<span data-ttu-id="23f1b-113">0</span><span class="sxs-lookup"><span data-stu-id="23f1b-113">0</span></span>|<span data-ttu-id="23f1b-114">Stellt eine Verbindung zum lokalen Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="23f1b-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="23f1b-115">gehostet</span><span class="sxs-lookup"><span data-stu-id="23f1b-115">hosted</span></span>|<span data-ttu-id="23f1b-116">1</span><span class="sxs-lookup"><span data-stu-id="23f1b-116">1</span></span>|<span data-ttu-id="23f1b-117">Stellt eine Verbindung mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="23f1b-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="23f1b-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="23f1b-118">serviceToService</span></span>|<span data-ttu-id="23f1b-119">2</span><span class="sxs-lookup"><span data-stu-id="23f1b-119">2</span></span>|<span data-ttu-id="23f1b-120">Intune Service verbindet direkt mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="23f1b-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="23f1b-121">dedizierte</span><span class="sxs-lookup"><span data-stu-id="23f1b-121">dedicated</span></span>|<span data-ttu-id="23f1b-122">3</span><span class="sxs-lookup"><span data-stu-id="23f1b-122">3</span></span>|<span data-ttu-id="23f1b-123">Stellt eine Verbindung zu Office 365 dedizierte Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="23f1b-123">Connects to O365 Dedicated Exchange environment.</span></span>|





