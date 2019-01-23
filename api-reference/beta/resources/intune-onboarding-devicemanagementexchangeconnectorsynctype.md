---
title: DeviceManagementExchangeConnectorSyncType Enum-Typ
description: Der Typ des Exchange-Connectors Synchronisierung angefordert.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a78bf79990eb16ae6dbc62d4c324b905a79a7f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405625"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="d0d7f-103">DeviceManagementExchangeConnectorSyncType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d0d7f-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="d0d7f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d0d7f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0d7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0d7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0d7f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0d7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0d7f-107">Der Typ des Exchange-Connectors Synchronisierung angefordert.</span><span class="sxs-lookup"><span data-stu-id="d0d7f-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="d0d7f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d0d7f-108">Members</span></span>
|<span data-ttu-id="d0d7f-109">Member</span><span class="sxs-lookup"><span data-stu-id="d0d7f-109">Member</span></span>|<span data-ttu-id="d0d7f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d0d7f-110">Value</span></span>|<span data-ttu-id="d0d7f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0d7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0d7f-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="d0d7f-112">fullSync</span></span>|<span data-ttu-id="d0d7f-113">0</span><span class="sxs-lookup"><span data-stu-id="d0d7f-113">0</span></span>|<span data-ttu-id="d0d7f-114">Entdecken Sie das Gerät im Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0d7f-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="d0d7f-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="d0d7f-115">deltaSync</span></span>|<span data-ttu-id="d0d7f-116">1</span><span class="sxs-lookup"><span data-stu-id="d0d7f-116">1</span></span>|<span data-ttu-id="d0d7f-117">Entdecken Sie nur das Gerät in Exchange die während des Delta Sync-Fensters aktualisiert haben.</span><span class="sxs-lookup"><span data-stu-id="d0d7f-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




