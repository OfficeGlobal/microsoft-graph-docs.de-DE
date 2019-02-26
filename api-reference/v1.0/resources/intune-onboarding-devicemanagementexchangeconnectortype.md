---
title: deviceManagementExchangeConnectorType-Enumerationstyp
description: Der Typ des Exchange-Connectors.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358832db83e5f5b3e1fb0f5457f480d21ded996
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263560"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="debf7-103">deviceManagementExchangeConnectorType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="debf7-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="debf7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="debf7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="debf7-105">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="debf7-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="debf7-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="debf7-106">Members</span></span>
|<span data-ttu-id="debf7-107">Element</span><span class="sxs-lookup"><span data-stu-id="debf7-107">Member</span></span>|<span data-ttu-id="debf7-108">Wert</span><span class="sxs-lookup"><span data-stu-id="debf7-108">Value</span></span>|<span data-ttu-id="debf7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="debf7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="debf7-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="debf7-110">onPremises</span></span>|<span data-ttu-id="debf7-111">0</span><span class="sxs-lookup"><span data-stu-id="debf7-111">0</span></span>|<span data-ttu-id="debf7-112">Stellt eine Verbindung mit der lokalen Exchange-Umgebung her.</span><span class="sxs-lookup"><span data-stu-id="debf7-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="debf7-113">gehostet</span><span class="sxs-lookup"><span data-stu-id="debf7-113">hosted</span></span>|<span data-ttu-id="debf7-114">1</span><span class="sxs-lookup"><span data-stu-id="debf7-114">1</span></span>|<span data-ttu-id="debf7-115">Verbindung zu O365-Exchange-Umgebung mit mehreren Mandanten</span><span class="sxs-lookup"><span data-stu-id="debf7-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="debf7-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="debf7-116">serviceToService</span></span>|<span data-ttu-id="debf7-117">2</span><span class="sxs-lookup"><span data-stu-id="debf7-117">2</span></span>|<span data-ttu-id="debf7-118">InTune-Dienst stellt eine direkte Verbindung zu O365-Exchange-Umgebung mit mehreren Mandanten her</span><span class="sxs-lookup"><span data-stu-id="debf7-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="debf7-119">dedizierten</span><span class="sxs-lookup"><span data-stu-id="debf7-119">dedicated</span></span>|<span data-ttu-id="debf7-120">3</span><span class="sxs-lookup"><span data-stu-id="debf7-120">3</span></span>|<span data-ttu-id="debf7-121">Stellt eine Verbindung zu einer dedizierten Exchange-Umgebung von O365 her.</span><span class="sxs-lookup"><span data-stu-id="debf7-121">Connects to O365 Dedicated Exchange environment.</span></span>|



