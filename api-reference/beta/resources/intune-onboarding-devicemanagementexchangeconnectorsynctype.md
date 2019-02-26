---
title: deviceManagementExchangeConnectorSyncType-Enumerationstyp
description: Der Typ der angeforderten Exchange-Connector-Synchronisierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47021a0a071995261f218cd4080026ababa33e0f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166598"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="7e31c-103">deviceManagementExchangeConnectorSyncType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="7e31c-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="7e31c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e31c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e31c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7e31c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e31c-106">Der Typ der angeforderten Exchange-Connector-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="7e31c-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="7e31c-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="7e31c-107">Members</span></span>
|<span data-ttu-id="7e31c-108">Element</span><span class="sxs-lookup"><span data-stu-id="7e31c-108">Member</span></span>|<span data-ttu-id="7e31c-109">Wert</span><span class="sxs-lookup"><span data-stu-id="7e31c-109">Value</span></span>|<span data-ttu-id="7e31c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e31c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e31c-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="7e31c-111">fullSync</span></span>|<span data-ttu-id="7e31c-112">0</span><span class="sxs-lookup"><span data-stu-id="7e31c-112">0</span></span>|<span data-ttu-id="7e31c-113">Entdecken Sie das gesamte Gerät in Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e31c-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="7e31c-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="7e31c-114">deltaSync</span></span>|<span data-ttu-id="7e31c-115">1</span><span class="sxs-lookup"><span data-stu-id="7e31c-115">1</span></span>|<span data-ttu-id="7e31c-116">Entdecken Sie nur das Gerät in Exchange, das während des Delta Sync-Fensters aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="7e31c-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




