---
title: deviceManagementExchangeConnectorType-Enumerationstyp
description: Der Typ des Exchange-Connectors.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8742a146f1183376424678f070b902eb052df5ac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150435"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="9e1f9-103">deviceManagementExchangeConnectorType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="9e1f9-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="9e1f9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e1f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e1f9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e1f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e1f9-106">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="9e1f9-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="9e1f9-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="9e1f9-107">Members</span></span>
|<span data-ttu-id="9e1f9-108">Element</span><span class="sxs-lookup"><span data-stu-id="9e1f9-108">Member</span></span>|<span data-ttu-id="9e1f9-109">Wert</span><span class="sxs-lookup"><span data-stu-id="9e1f9-109">Value</span></span>|<span data-ttu-id="9e1f9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e1f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e1f9-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="9e1f9-111">onPremises</span></span>|<span data-ttu-id="9e1f9-112">0</span><span class="sxs-lookup"><span data-stu-id="9e1f9-112">0</span></span>|<span data-ttu-id="9e1f9-113">Stellt eine Verbindung mit der lokalen Exchange-Umgebung her.</span><span class="sxs-lookup"><span data-stu-id="9e1f9-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="9e1f9-114">gehostet</span><span class="sxs-lookup"><span data-stu-id="9e1f9-114">hosted</span></span>|<span data-ttu-id="9e1f9-115">1</span><span class="sxs-lookup"><span data-stu-id="9e1f9-115">1</span></span>|<span data-ttu-id="9e1f9-116">Verbindung zu O365-Exchange-Umgebung mit mehreren Mandanten</span><span class="sxs-lookup"><span data-stu-id="9e1f9-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="9e1f9-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="9e1f9-117">serviceToService</span></span>|<span data-ttu-id="9e1f9-118">2</span><span class="sxs-lookup"><span data-stu-id="9e1f9-118">2</span></span>|<span data-ttu-id="9e1f9-119">InTune-Dienst stellt eine direkte Verbindung zu O365-Exchange-Umgebung mit mehreren Mandanten her</span><span class="sxs-lookup"><span data-stu-id="9e1f9-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="9e1f9-120">dedizierten</span><span class="sxs-lookup"><span data-stu-id="9e1f9-120">dedicated</span></span>|<span data-ttu-id="9e1f9-121">3</span><span class="sxs-lookup"><span data-stu-id="9e1f9-121">3</span></span>|<span data-ttu-id="9e1f9-122">Stellt eine Verbindung zu einer dedizierten Exchange-Umgebung von O365 her.</span><span class="sxs-lookup"><span data-stu-id="9e1f9-122">Connects to O365 Dedicated Exchange environment.</span></span>|




