---
title: DeviceManagementExchangeConnectorType Enum-Typ
description: Der Typ des Exchange-Connectors.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20eb1053d3dbf6cb657313f0c68f6c6c84804848
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398982"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="a1d33-103">DeviceManagementExchangeConnectorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a1d33-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="a1d33-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a1d33-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1d33-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1d33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1d33-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1d33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1d33-107">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="a1d33-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="a1d33-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a1d33-108">Members</span></span>
|<span data-ttu-id="a1d33-109">Member</span><span class="sxs-lookup"><span data-stu-id="a1d33-109">Member</span></span>|<span data-ttu-id="a1d33-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a1d33-110">Value</span></span>|<span data-ttu-id="a1d33-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1d33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1d33-112">"lokal"</span><span class="sxs-lookup"><span data-stu-id="a1d33-112">onPremises</span></span>|<span data-ttu-id="a1d33-113">0</span><span class="sxs-lookup"><span data-stu-id="a1d33-113">0</span></span>|<span data-ttu-id="a1d33-114">Stellt eine Verbindung zum lokalen Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="a1d33-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="a1d33-115">gehostet</span><span class="sxs-lookup"><span data-stu-id="a1d33-115">hosted</span></span>|<span data-ttu-id="a1d33-116">1</span><span class="sxs-lookup"><span data-stu-id="a1d33-116">1</span></span>|<span data-ttu-id="a1d33-117">Stellt eine Verbindung mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="a1d33-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="a1d33-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="a1d33-118">serviceToService</span></span>|<span data-ttu-id="a1d33-119">2</span><span class="sxs-lookup"><span data-stu-id="a1d33-119">2</span></span>|<span data-ttu-id="a1d33-120">Intune Service verbindet direkt mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="a1d33-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="a1d33-121">dedizierte</span><span class="sxs-lookup"><span data-stu-id="a1d33-121">dedicated</span></span>|<span data-ttu-id="a1d33-122">3</span><span class="sxs-lookup"><span data-stu-id="a1d33-122">3</span></span>|<span data-ttu-id="a1d33-123">Stellt eine Verbindung zu Office 365 dedizierte Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="a1d33-123">Connects to O365 Dedicated Exchange environment.</span></span>|




